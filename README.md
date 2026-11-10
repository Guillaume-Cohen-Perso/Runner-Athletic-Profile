# Runner-Athletic-Profile
## Running Profile & Performance Predictor 🏃‍♂️⚡

A lightweight, zero-dependency, single-page web application designed for runners and coaches to model physiological profiles, energy expenditure, heart rate zones, and race performances.
It can be directly seen here : [Runner Athletic Profile](https://guillaume-cohen-perso.github.io/Runner-Athletic-Profile/)

![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)
![HTML5/CSS3/JS](https://img.shields.io/badge/tech-HTML5%20%2F%20CSS3%20%2F%20JS-orange)

## Features

- **Physiological Profiling**: Calculates effective $\text{VO}_2\text{max}$, VDOT (Jack Daniels), Maximum Aerobic Speed (MAS / VMA), Critical Speed (CS / VC), and Critical Power (CP & $W'$).
- **Incline & Energetics**: Estimates metabolic power (Watts), mechanical power, and energy cost per km based on gradient (%) using the Minetti et al. (2002) model.
- **Heart Rate & Training Zones**:
  - Heart rate zones (Karvonen vs. % HRmax).
  - MAS / VMA pacing zones.
  - Critical Speed / Critical Power zones.
- **Race Predictions**: Compares multiple modeling approaches:
  - **Daniels VDOT** (physiological equivalent).
  - **Adjusted Riegel** (with exponent $k$ dynamically fitted to the runner's level).
  - **CNRS/MIT Logarithmic Model** ($v(T) = a + b \ln T$).
  - **Critical Speed / $W'$** (distance-limited model).
- **Interactive HR vs. Distance Chart**: SVG-based dynamic chart allowing real-time dragging of target distance and heart rate.
- **Formulas & References**: Includes a complete collapsible appendix with equations and scientific literature references.

## Getting Started

No setup, build steps, or external packages are required!

1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/running-profile-calculator.git
   ```
2. Open `index.html` in any web browser.

## Project Structure

```text
├── index.html   # Main application structure, scripts, and layout
├── style.css    # Responsive grid layout and CSS variable themes
└── README.md    # Documentation
```

## Scientific References

- **Minetti et al. (2002)**: Energy cost of walking and running at extreme slopes.
- **Daniels & Gilbert (1979)**: VDOT and oxygen consumption formulas.
- **Monod & Scherrer (1965)**: Critical Power concept.
- **Riegel (1981) / Cameron (1999)**: Performance decay and level-adjusted exponents.
- **Mulligan, Adam & Emig (2018)**: CNRS / MIT logarithmic running performance model (PLoS ONE).
- **Karvonen et al. (1957) / Swain et al. (1994)**: Heart rate reserve and % HRmax conversions.

## License

Copyright 2026

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
