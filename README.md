# acer-keyboard-debugger
Minimal PowerShell scripts to detect Fn-Lock and keyboard layout mismatches on Windows
How to use

Open PowerShell (Win+X → Windows PowerShell).

Paste List-KeyboardLayouts.ps1 → check if a Dvorak/Intl layout is silently present.

Paste KeyViewer.ps1 → press the top row keys. If 0 yields /, you’ll see it immediately.

For laptops with Fn-Lock: try Fn+Esc (Acer), or toggle in BIOS (Action Keys / Fn Lock). Software can’t reliably flip Fn-Lock.

Why this helps

Surfaces hidden OS layouts that hijack digits (e.g. Dvorak prints symbols without Shift).

Confirms the physical board vs. OS layout mismatch (US vs. UK vs. localized variants).

Gives reproducible data (VK codes, chars) for bug reports.

Looking for feedback

Other vendor Fn-Lock combos to document?

Safe heuristics to suggest an OS layout reset without touching the registry?

Edge cases (embedded numpad, swapped Ctrl/Fn, US-Intl dead keys) worth adding?

Early stage, but this triage flow immediately explained my Acer issue and let me type again without holding Fn with one hand.
