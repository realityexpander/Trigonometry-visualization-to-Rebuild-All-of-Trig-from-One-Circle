# One Circle, Six Functions, Three Phases

**An interactive visualization of trigonometry built from the unit circle.** Explore all six trigonometric functions, their geometric relationships, the three Pythagorean identities, and the sine/cosine angle-addition formulas.

<img width="600" alt="image" src="https://github.com/user-attachments/assets/d8b8acfb-cc5a-4a24-a58f-d7b6b6e7fa33" />


[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

**Source video:** [You Can Rebuild All of Trig From This One Circle](https://www.youtube.com/watch?v=mOBWUJwaJ9k)  
**Source code:** [GitHub repository](https://github.com/realityexpander/Trigonometry-visualization-to-Rebuild-All-of-Trig-from-One-Circle)

## Features

- **Three independent learning phases** with selectable tabs.
- **Six independently visible trigonometric functions:** sine, cosine, tangent, cotangent, secant, and cosecant. Show any combination, including all six simultaneously.
- **Four selectable quadrants (I–IV).** Switch quadrants while preserving the acute reference angle, or drag the unit-circle point between quadrants.
- **Live numerical values** and color-coded SVG diagrams that update as the angle changes.
- **Angle slider, ±1° buttons, and reset** (38° reference angle) in Phases 1 and 2.
- **Function presets:** Shadow, Touch, Cut, All six, and None.
- **Three optional Pythagorean triangles**, each independently visible in Phase 2.
- **Independent A and B angle controls** and height/width component views in Phase 3.
- **Runs offline:** a single HTML file with embedded CSS and JavaScript; no installation, frameworks, or external runtime dependencies.
- Chat that generated the app: https://chatgpt.com/share/6ad4e634-3574-83e9-837e-84b14572a3ba

## Getting started

1. Download or clone this repository.
2. Open `interactive_unit_circle.html` directly in a modern browser (Chrome, Firefox, Edge, or Safari).
3. Select a phase and interact with the controls. No web server is required.

```bash
git clone https://github.com/realityexpander/Trigonometry-visualization-to-Rebuild-All-of-Trig-from-One-Circle.git
cd Trigonometry-visualization-to-Rebuild-All-of-Trig-from-One-Circle
```

Then open `interactive_unit_circle.html` in your browser. You can also host the file on a static web server, including GitHub Pages; use `index.html` as the entry point if needed.

## Phase 1 — The three physical actions

The video describes three geometric actions applied in two directions, giving six trigonometric functions:

| Physical action | Horizontal construction | Vertical construction |
| --- | --- | --- |
| **Shadow** (projection) | **cos θ**: horizontal projection | **sin θ**: vertical projection |
| **Touch** (tangent line) | **cot θ**: segment along the horizontal tangent line | **tan θ**: segment along the vertical tangent line |
| **Cut** (ray meeting a tangent) | **csc θ**: segment to the horizontal tangent line | **sec θ**: segment to the vertical tangent line |

Use the six checkboxes to isolate a single function or compare multiple constructions. The colored tangent and secant segments depict **nonnegative geometric lengths**; the numeric readouts reflect the **signed function values** in the selected quadrant.

### Quadrant controls

Select **I**, **II**, **III**, or **IV** using the buttons above the angle slider. The current reference angle is preserved: for example, 38° in Quadrant I corresponds to 142°, 218°, and 322° in Quadrants II, III, and IV.

| Quadrant | sin / csc | cos / sec | tan / cot |
| --- | :---: | :---: | :---: |
| I | + | + | + |
| II | + | − | − |
| III | − | − | + |
| IV | − | + | − |

To avoid undefined ratios and excessively long line segments near the axes, the angle controls keep the ray at least 8° from a quadrant boundary. The displayed angles are therefore limited to 8°–82°, 98°–172°, 188°–262°, and 278°–352°.

## Phase 2 — The three scales of Pythagoras

Enable any of the three right-triangle constructions individually or together:

1. **Inside the unit circle:** `sin² θ + cos² θ = 1`
2. **At the vertical tangent:** `1 + tan² θ = sec² θ`
3. **At the horizontal tangent:** `1 + cot² θ = csc² θ`

All three are versions of the Pythagorean theorem, `a² + b² = c²`, at different geometric scales. The squared identities hold in all four quadrants.

## Phase 3 — Interaction and the angle-addition payoff

Change angles **A** and **B** independently, with their sum restricted to at most 85° to keep the illustrated geometry in the first quadrant. Choose **Both**, **Sine / height**, or **Cosine / width** to examine the contributing segments.

**Vertical height:**

```text
sin(A + B) = sin(A)cos(B) + cos(A)sin(B)
```

**Horizontal width:**

```text
cos(A + B) = cos(A)cos(B) − sin(A)sin(B)
```

The negative term in the cosine identity is visualized as the horizontal component pointing backwards.

> Phase 3 is a **first-quadrant geometric illustration** of angle addition, separate from the four-quadrant controls in Phases 1 and 2.

## Project files

```text
.
├── interactive_unit_circle.html  # Complete standalone application
├── README.md                     # Project information and usage
└── LICENSE                       # MIT license
```

## Technology

- HTML5
- CSS3
- JavaScript (vanilla)
- SVG for the interactive constructions

No package manager, build step, or framework is required.

## Video inspiration and attribution

This project is an interactive exploration of the geometry illustrated in the video [**You Can Rebuild All of Trig From This One Circle**](https://www.youtube.com/watch?v=mOBWUJwaJ9k), using the three-phase approach:

1. The three physical actions — shadow, touch, and cut.
2. The three scales of Pythagoras.
3. Interactions that reveal the angle-addition formulas.

The video is credited as the **source of the educational presentation**; the MIT license below applies to this repository's code, not to the source video's material.

## License

This project is distributed under the **MIT License**. See [`LICENSE`](LICENSE) for the full license text.

**Copyright © 2026 Chris Athanas.**

[GitHub Source](https://github.com/realityexpander/Trigonometry-visualization-to-Rebuild-All-of-Trig-from-One-Circle)
