# 🖥️ Tkinter Mini Projects

A collection of mini projects built using **Python and Tkinter** — Python's built-in GUI library. Each project is self-contained in its own folder with its own code and documentation.

---

## 📋 Table of Contents

- [About Tkinter](#about-tkinter)
- [Projects](#projects)
- [Requirements](#requirements)
- [How to Run Any Project](#how-to-run-any-project)
- [Repository Structure](#repository-structure)
- [Author](#author)

---

## 🪟 About Tkinter

`tkinter` is Python's standard GUI (Graphical User Interface) library. It comes **built into Python** — no separate installation needed. It allows developers to build desktop applications with windows, buttons, labels, entry boxes, and more.

---

<!-- PROJECTS_START -->
## 🗂️ Projects

| Project | Description | Key Libraries |
|---|---|---|
| [🧮 GUI Calculator](./GUI_calculator/README.md) | A dark-themed desktop calculator with safe expression evaluation and chained calculation support | `tkinter`, `simpleeval` |
| [🧒 Kids Games](./kids_games/README.md) | An interactive educational quiz app for kids covering Math, GK, and Spelling with score tracking | `tkinter`, `simpleeval`, `random` |

<!-- PROJECTS_END -->

---

## 🛠️ Requirements

- Python 3.6+
- `tkinter` — built into Python, no install needed
- [`simpleeval`](https://pypi.org/project/simpleeval/) — used by both projects

Install all dependencies at once:
```bash
pip install simpleeval
```

---

## 🚀 How to Run Any Project

1. Navigate into the project folder:
   ```bash
   cd GUI_calculator
   # or
   cd kids_games
   ```

2. Run the Python file:
   ```bash
   python calculator.py
   # or
   python kids_game.py
   ```

---

## 📁 Repository Structure

```
tkinter-projects/
│
├── README.md                          ← You are here (parent README)
│
├── GUI_calculator/
│   ├── calculator.py                  ← Calculator source code
│   └── README.md                      ← Calculator documentation
│
└── kids_games/
    ├── kids_game.py                   ← Kids game source code
    └── README.md                      ← Kids game documentation
```

---

## 👤 Author

- **Dadi Rohit** — [DadiRohit45](https://github.com/DadiRohit45)

---

## 📄 License

This repository is open-source and available under the [MIT License](LICENSE).
