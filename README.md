# GdScO₃ Photoluminescence Analysis (trace Eu³⁺)

Interactive and scripted analysis of excitation-dependent photoluminescence (PL) 
in nominally undoped GdScO₃ single crystals that contain trace (1–2 ppm) Eu³⁺, comparing two crystal samples 
(Crystal A — Amazon, Crystal B — Bharat).

## Contents

| File | Description |
|---|---|
| `Amazon vs Bharat_PL.html` | Interactive Plotly visualization — open in any browser |
| `Amazon vs Bharat_PL.py` | Python script for stacked PL plots with draggable excitation/emission lines |

## Live Interactive Plot

[Open the interactive PL viewer](https://shadi-mirmohammadi.github.io/gso-pl-analysis/Amazon%20vs%20Bharat_PL.html)
No installation needed — runs directly in your browser.

## Science

Tuning the excitation from 250 to 263 nm lowers the 491/612 nm emission line ratio from 1.03 to 0.13 in Crystal A.
No Eu³⁺ emission is detected for excitation from 276 to 288 nm, the range that covers the Gd³⁺ ⁸S₇/₂ → ⁶I_J absorption lines.

Crystal A (Amazon) and Crystal B (Bharat) are compared across the full 
excitation-emission landscape to probe site symmetry, energy transfer 
efficiency, and defect contributions.

## Python Script

### Requirements

```bash
pip install pandas matplotlib numpy openpyxl
```

### Usage

Place `Amazon vs Bharat_PL.py` in the same folder as your `.xlsx` data files 
(dark spectrum, transmission spectrum, and individual PL files named by 
excitation wavelength, e.g. `254 nm.xlsx`), then run:

```bash
python "Amazon vs Bharat_PL.py"
```

Drag the red dashed line on the transmission panel to select an excitation 
wavelength — the corresponding PL spectrum highlights automatically.
Line positions are saved between sessions.

## Author

Shadi Mirmohammadi  
Ph.D. student, Electrical & Computer Engineering, University of Utah  
Sensale-Rodriguez Lab
