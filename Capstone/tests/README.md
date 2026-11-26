# Testing

## 1. Tests that were actually run

From the `capstone/` folder:

```powershell
python -m unittest discover -s tests -v
```

Result at the time of writing: **33 tests passed**.

| Test file | What it checks | Result |
|---|---|---|
| `test_assembler.py` | Official C-instruction encoding, A-instruction limits, predefined symbols, error messages with source line numbers, `symbols.txt` grouping, and comparison against official symbol-less programs | Passed |
| `test_box.py` | Runs `Box.hack` in a small Python reference Hack interpreter; verifies no writes when idle, exactly 80 black words on key press, exactly 80 white words on key release, and no writes outside the box | Passed |
| `test_hdl_static.py` | HDL file structure (chip name, braces, required parts), address calculations, and 16-bit width of every generated `.hack` file | Passed |

### Assembler comparison note

The official Nand2Tetris assembler program was **not available in this workspace**, so a direct comparison against the official assembler was **not performed**.

Instead, the following official files were downloaded from the Nand2Tetris GitHub repository:

- `programs/Add.asm`, `programs/Max.asm`, `programs/Rect.asm`, `programs/Pong.asm`
- `tests/reference/MaxL.asm`, `tests/reference/RectL.asm`, `tests/reference/PongL.asm`

Each symbolic program was assembled and compared byte-for-byte with its official symbol-less (`*L.asm`) version. All three comparisons passed. This verifies label addresses, variable addresses (starting at RAM 16), and C-instruction encoding against official source data.

## 2. HDL tests provided but not run

The official Hardware Simulator test scripts were downloaded into:

```text
tests/official-hdl-tests/
```

They include:

- `CPU.tst` / `CPU.cmp`
- `Memory.tst` / `Memory.cmp`
- `ComputerAdd.tst` / `ComputerAdd.cmp`
- `ComputerMax.tst` / `ComputerMax.cmp`
- `ComputerRect.tst` / `ComputerRect.cmp`

The Nand2Tetris **Hardware Simulator is not installed in this workspace**, so these scripts could not be executed here. Do not claim they passed until you run them yourself.

### Running them manually

1. Install the official Nand2Tetris tools from <https://www.nand2tetris.org/software>.
2. Copy `CPU.hdl`, `Memory.hdl`, and `Computer.hdl` from `capstone/` into `capstone/tests/official-hdl-tests/`. (The `.tst` scripts use `load CPU.hdl`, etc., so the HDL files must sit beside them.)
3. Start the Hardware Simulator.
4. Open `tests/official-hdl-tests/CPU.tst` and run it. Compare with `CPU.cmp`.
5. Repeat for `Memory.tst`, `ComputerAdd.tst`, `ComputerMax.tst`, and `ComputerRect.tst`.
6. Capture a screenshot for each script that ends with "End of script - Comparison ended successfully".

## 3. Box.hack testing

`Box.hack` was executed in the Python reference interpreter inside `test_box.py`, not in the official CPU Emulator. The CPU Emulator was not available in this workspace.

For manual verification in the official CPU Emulator:

1. Open the CPU Emulator.
2. Load `Box.hack`.
3. Select the screen view and the keyboard input.
4. Leave the keyboard at 0 and run the program: the box area must stay white.
5. Press any key: a black rectangle should appear at row 87, 20 rows high and 64 pixels wide, starting at the left edge.
6. Release the key: the rectangle should disappear.
7. Confirm no other part of the screen changes.

See `screenshots/README.md` for the exact screenshot checklist.
