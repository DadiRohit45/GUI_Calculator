# 🧮 GUI_Calculator

A sleek, dark-themed desktop calculator built with **Python and Tkinter**, featuring safe expression evaluation using `simpleeval` and smooth chained calculation support.

---

## 📋 Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Button Layout](#button-layout)
- [Code Overview](#code-overview)
- [Known Limitations](#known-limitations)
- [Future Improvements](#future-improvements)

---

## ✨ Features

- 🖤 **Dark themed UI** — black background with orange operator highlights
- ➕ **Basic arithmetic** — addition, subtraction, multiplication, division
- 💯 **Percentage support** — `%` operator included
- 🔢 **Decimal support** — `.` button for floating point numbers
- 🔗 **Chained calculations** — continue calculating from the last result
- ⌫ **Backspace** — delete last entered character
- 🔄 **AC (All Clear)** — clears the entire expression and resets state
- 📐 **Euler's number** — `e` button for mathematical constant `2.718281828`
- ✅ **Safe evaluation** — uses `simpleeval` instead of `eval()`
- 🖱️ **Hand cursor** — cursor changes on button hover for better UX

---

## 🛠️ Requirements

- Python 3.6+
- [`simpleeval`](https://pypi.org/project/simpleeval/) — safe math expression evaluator
- `tkinter` — built into Python (no separate install needed)

---

## 📦 Installation

1. **Clone or download** the repository:
   ```bash
   git clone https://github.com/your-username/tkinter-calculator.git
   cd tkinter-calculator
   ```

2. **Install dependencies:**
   ```bash
   pip install simpleeval
   ```

3. **Run the program:**
   ```bash
   python calculator.py
   ```

---

## 🚀 Usage

1. Launch the app — a dark-themed calculator window opens.
2. Click number buttons to enter digits.
3. Click operator buttons (`+`, `—`, `x`, `/`, `%`) to add operations.
4. Click `=` to evaluate and see the result.
5. After `=`, you can **continue calculating from the result** by pressing any operator.
6. Click `⌫` to delete the last character.
7. Click `AC` to clear everything and start fresh.

### Example — Chained Calculation
```
Press: 5 + 3 =   → shows 8
Press: + 2 =      → shows 10   ✅ continues from 8
Press: * 3 =      → shows 30   ✅ continues from 10
```

---

## 🔢 Button Layout

```
┌─────────────────────────────┐
│        [ Display ]          │  ← Entry (black bg, white text)
├──────┬──────┬──────┬────────┤
│  7   │  8   │  9   │   /   │
├──────┼──────┼──────┼────────┤
│  4   │  5   │  6   │   —   │
├──────┼──────┼──────┼────────┤
│  1   │  2   │  3   │   +   │
├──────┼──────┼──────┼────────┤
│  0   │  •   │  x   │   %   │
├──────┼──────┼──────┼────────┤
│  e   │  =   │  AC  │   ⌫   │
└──────┴──────┴──────┴────────┘
```

---

## 🗂️ Code Overview

| Function | Description |
|---|---|
| `click(a)` | Appends clicked value to expression and updates display |
| `calculation()` | Safely evaluates expression using `simpleeval` and shows result |
| `clear()` | Clears display, resets expression and `result_shown` flag |
| `remove()` | Deletes the last character from display and expression |

### How Chained Calculation Works (`result_shown` flag)

```
User presses 5 + 3
  → expression = "5+3"

User presses =
  → result = "8"
  → expression = "8"
  → result_shown = True

User presses +
  → result_shown is True → clear display only
  → result_shown = False
  → expression = "8+"    ← continues from result ✅

User presses 2 =
  → result = "10"        ✅
```

The `result_shown` flag clears the **display** after `=` while keeping the **expression** intact, allowing seamless chained calculations.

---

## 🔐 Security Note

This calculator uses `simpleeval` instead of Python's built-in `eval()` for safe expression evaluation. `simpleeval` only allows mathematical operations and blocks any attempt to execute system commands or import modules.

```python
# ❌ Unsafe
result = eval(expression)

# ✅ Safe
result = simple_eval(expression)
```

---


---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

- [`simpleeval`](https://pypi.org/project/simpleeval/) for safe math expression evaluation
- Python's built-in `tkinter` for the GUI framework
