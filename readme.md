## Horizon Extended 2026 - Dark Theme for Visual Studio 2026

**Horizon Extended 2026** is a Visual Studio 2026 port of the **Horizon Extended** VS Code theme, matching the editor, UI, and terminal colors as closely as VS allows.

---

## Repository Contents

```
build_vsix.py            - Python script that builds a .vsix theme from the YAML config
HorizonExtended2026.yaml - Theme configuration
HorizonExtended2026.png  - Theme icon image
HorizonExtended2026.vsix - Built VSIX (ready to install)
```

---

## Building the VSIX

Requires **Python 3.8+** and the **PyYAML** library.

1. Install dependency:

```sh
pip install pyyaml
```

2. Build the theme:

```sh
python build_vsix.py -i HorizonExtended2026.yaml -o HorizonExtended2026
```

This produces:

```
HorizonExtended2026.vsix
```

---

## Installing in Visual Studio

1. Close Visual Studio.
2. Double-click `HorizonExtended2026.vsix` and complete the installer.
3. Reopen Visual Studio.
4. Select the theme:
   Tools > Theme (or Tools > Options > Environment > General > Color theme).

---

## Customizing

Edit:

```
HorizonExtended2026.yaml
```

Then rebuild:

```sh
python build_vsix.py -i HorizonExtended2026.yaml -o HorizonExtended2026
```

---

## Credits

* Based on the **Horizon Extended** VS Code theme.
