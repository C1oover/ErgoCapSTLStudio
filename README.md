# ErgoCap STL Studio

A browser-based tool for customizing sculpted ergonomic keycaps (KLP Lamé, CLP, Chicago Stenographer, or any local `.stl`) without losing the original surface geometry. Runs entirely client-side as a single `index.html` file on GitHub Pages.

## Features

- **Uses Exact Open-Source STLs:** Pulls the original binary `.stl` files directly from `braindefender/KLP-Lame-Keycaps`, `vvhg1/clp-keycaps`, `rschenk/cfx_chicago_stenographer`, or any custom GitHub repository / local `.stl` file.
- **Pitch, Roll & Explicit Height Lofting:** Tilts (up/down and left/right) and adjusts the height of the top dish while smoothly lofting the side walls down to a flat horizontal skirt plane (`C¹` Hermite lofting with no bezel lip at steep angles). The switch stem stays vertical and anchored at the native stem seat datum.
- **Choc v1 Ambient Switch Clearance (No Spacers Needed):** Trims the bottom skirt rim upward (`+0.4` to `+0.6 mm`) and adjusts prong tip length while keeping the stem seat and top dish at their original height—preventing bottom-out collisions on Kailh Choc Ambient switches (Twilight / Nocturnal / Sunrise) or MoErgo without plastic spacers or added key height.
- **Homing Reliefs & Arbitrary Legends (Protruding or Recessed):** Adaptive top-surface subdivision (`0.12 mm` resolution) + 2D Signed Distance Fields for adding bars, dots, rings, or arbitrary letters/symbols as either raised bumps (`+`) or engraved scoops (`-`).
- **Socket Swapping & 3D Print Tolerances:** Fine-tune stem XY fit tolerances on the native STL stem, or swap the socket between Choc v1 (`0°` / `90°`) and Cherry MX.

## Usage / Local Run

No build step or dependencies required. Open `index.html` in any browser, or host directly via GitHub Pages
