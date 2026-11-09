# 03 — Debounce

A single noisy OPEN frame should not trigger an action. The example requires N consecutive identical valid classifications before accepting a state change. Invalid/WAITING input resets the streak.

Run:
```bash
python 03_debounce/debounce_demo.py
```
