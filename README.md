# smartpi-wheels

Pre-built Python wheels for the Yumi Smart Pi One / SmartPad
(Allwinner H3, **armv7l 32-bit**, uv-managed CPython 3.13).

These are the C-extension packages that have **no upstream armv7l wheel** and
would otherwise compile from source on the board (20-40 min each, and hot).
Built once on real hardware, hosted here, and pulled by the YUMI OS Board
CLI installers via `--find-links`, so a 1-click install downloads in seconds
instead of compiling.

## Use

```bash
uv tool install <pkg> --find-links https://yumi-lab.github.io/smartpi-wheels/
# or, without Pages:
uv pip install <pkg> --find-links https://raw.githubusercontent.com/Yumi-Lab/smartpi-wheels/main/index.html
```

`UV_FIND_LINKS` is honoured too.

## Contents (release `v1`)

Harvested from a real `uv` build on the Smart Pi One. Tags: `cp313-cp313-linux_armv7l`.

| package | version |
|---------|---------|
| cffi | 2.1.1 |
| httptools | 0.8.0 |
| markupsafe | 3.0.3 |
| pillow | 12.2.0 |
| pyyaml | 6.0.3 |
| regex | 2026.7.19 |
| setproctitle | 1.3.7 |
| uvloop | 0.22.1 |
