The "Calculator" Python script creates a simple graphical calculator application using the Tkinter library. Here's a breakdown of the key components and functionality:

1. Import and Window Setup:
- tkinter is imported as tk.
- The main application window (root) is created, titled "Calculator".
- The background color of the window is set to a dark shade (#2b2b2b).

2. Display:
- A StringVar named "display" holds the current input or result shown on screen.
- Initially, display is empty.
- A Label widget displays the content of "display" with white text on dark background, large font size, right-aligned.

3. Functions for Calculator Operations:
- append_to_display(value): Adds the clicked button’s value (number or operator) to the display.
- clear_display(): Clears the display, effectively resetting input.
- evaluate_expression(): Attempts to evaluate the arithmetic expression in the display using Python's eval().
  - If successful, it updates display with the result.
  - If an error occurs (invalid input), it sets the display to "Invalid Input".
- on_key_press(event): Handles keyboard input.
  - Accepts digits and operators (+, -, *, /, .) and appends them to display.
  - Pressing Enter ('Return') triggers evaluation.
  - Pressing Escape ('Escape') clears the display.

4. Buttons:
- Buttons are created for digits (0-9), decimal point ('.'), arithmetic operators (+, -, *, /), equals ('='), and a special button labeled 'A'.
- Button colors:
  - Regular buttons have a grey-blue background (#607d8b) and red text.
  - Special buttons (equals) have an orange background (#ff5722) and red text.
- The equals button triggers expression evaluation.
- Other buttons append their text to the display.
- Buttons are arranged in a grid layout.

5. Grid Layout Configuration:
- Rows and columns of the window grid are configured to expand evenly, ensuring responsive resizing.

6. Keyboard Bindings:
- The root window listens for key presses and processes them via on_key_press(), enabling keyboard input for calculator operations.

7. Main Loop:
- The Tkinter event loop starts with root.mainloop(), displaying the window and waiting for user interaction.

Overall, this script implements a basic functional calculator with a graphical interface that supports both mouse clicks and keyboard input for entering expressions and obtaining results.
