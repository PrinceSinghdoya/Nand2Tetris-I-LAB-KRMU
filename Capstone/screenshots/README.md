# Screenshot checklist

No screenshots are included in this folder. The Nand2Tetris Hardware Simulator and CPU Emulator were not available in the workspace, so no genuine simulator screenshots could be captured. Do not create fake screenshots.

Capture the following yourself after installing the official tools from <https://www.nand2tetris.org/software>.

| # | Screenshot to capture | Where / what to show |
|---|---|---|
| 1 | CPU test passed | Hardware Simulator running `CPU.tst`; bottom panel shows `End of script - Comparison ended successfully` |
| 2 | Memory test passed | Hardware Simulator running `Memory.tst` with the same success message |
| 3 | ComputerAdd test passed | Hardware Simulator running `ComputerAdd.tst` with the same success message |
| 4 | ComputerMax test passed | Hardware Simulator running `ComputerMax.tst` with the same success message |
| 5 | ComputerRect test passed | Hardware Simulator running `ComputerRect.tst` with the same success message |
| 6 | Assembler execution | Terminal showing `python assembler.py Box.asm` and the "Assembled ..." message |
| 7 | `symbols.txt` generated | Editor or terminal showing `SYMBOL TABLE`, `Labels:`, `Variables:` and entries such as `DRAW_ROW -> ...` and `row -> 16` |
| 8 | Box displayed in CPU Emulator | CPU Emulator screen view with a black 64 x 20 rectangle starting at row 87 while a key is held |
| 9 | Box disappearing after key release | Same CPU Emulator screen view after the key is released, showing the box area white again |

## Suggested file names

When you capture them, save them here using names like:

```text
screenshots/01_cpu_test_passed.png
screenshots/02_memory_test_passed.png
screenshots/03_computer_add_test_passed.png
screenshots/04_computer_max_test_passed.png
screenshots/05_computer_rect_test_passed.png
screenshots/06_assembler_execution.png
screenshots/07_symbols_txt.png
screenshots/08_box_pressed.png
screenshots/09_box_released.png
```

## Reminder

Only replace this README with real screenshots after you have actually run the simulators. If a screenshot cannot be captured, keep this checklist and explain why in your submission.
