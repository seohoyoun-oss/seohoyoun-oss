# Hi 👋, I'm Seoho

**Engineer who writes the tools that turn complex systems into decisions.**

Systems validation and optical engineer. I build Python tools to model and validate sensors based on physics, and full-stack applications that bring AI into hardware program management workflows.

---

## Software Tools

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic_API-CC785C?style=for-the-badge&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)
![Mathematica](https://img.shields.io/badge/Mathematica-DD1100?style=for-the-badge&logo=wolframmathematica&logoColor=white)
![JMP](https://img.shields.io/badge/JMP-005AA7?style=for-the-badge&logo=sas&logoColor=white)
![Imatest](https://img.shields.io/badge/Imatest-2C7BB6?style=for-the-badge&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

## Featured Projects

### [Dynamic Program Visualization](https://github.com/seohoyoun-oss/epm-tool-dynamic-visualization) · [Live Demo](https://epm-tool-dynamic-visualization.vercel.app)

An AI-powered program schedule tool for hardware program managers — a Gantt chart that thinks. Every task carries a live risk score recomputed on every edit; inject an issue and the AI identifies which tasks are affected, previews the schedule and health-metric impact before you commit, and proposes three mitigation paths with trade-offs that can be applied in one click.

Built around a real-world pain point: issues surface without warning, teams scramble, and alignment breaks down. This tool makes the impact visible instantly and gives the program manager a structured, AI-assisted process to recover. The demo program is an 18-month robot vacuum launch — 27 tasks across 10 phases, from concept through EVT/DVT/PVT to mass-production ramp.

**Stack:** Next.js 16 · TypeScript · Tailwind CSS · Zustand + Immer · Framer Motion · Custom SVG Gantt · Anthropic API (`claude-sonnet-4-6`) · jsPDF + SheetJS · Vercel

- Custom SVG Gantt with drag-to-move/resize bars, snapping to hardware-style B/M/E (1st/11th/21st) date boundaries
- Live risk scoring per task plus a program health dashboard (confidence, max slip, critical/at-risk/on-track counts)
- AI-identified affected tasks on issue entry, with hover preview of the full schedule impact before applying
- AI Risk Navigator: three mitigation options with trade-offs and a recommended path, committable in one click
- Streaming, on-demand AI schedule audit covering risk blind spots, owner conflicts, and schedule compression
- Export to 8 formats: PNG, SVG, PDF, CSV, XLSX, and MS Project (MSPDI XML, MPP, MPX)
- Hardened AI routes — retry budget, hard stream abort, bounded findings, and sanitized error surfacing

---

### [AI-Powered FMEA Assistant](https://github.com/seohoyoun-oss/epm-tool-fmea) · [Live Demo](https://epm-tool-fmea-qkrh.vercel.app)

A full-stack web application that accelerates Failure Mode and Effects Analysis for hardware program managers. Enter a design change description; the tool generates a structured FMEA table, ranks rows by Risk Priority Number, and plots them on an Action Priority Matrix mapping risk against implementation cost.

Built after running FMEA reviews on depth-sensing modules — the bottleneck on quality was always PM experience. The goal: compress that experience gap with a language model.

**Stack:** React 18 · Vite · Tailwind CSS · Anthropic API (`claude-sonnet-4-6`) · Vercel serverless · PapaParse · html2canvas

- Four-step workflow — review the preloaded Engineering Requirements Specification, enter the design change, generate, review and export
- Prompt scoped to failure modes introduced by the stated design change, not a generic system survey
- Editable table showing the top 10 rows by RPN, with scores clamped to 1–10 and live RPN recalculation
- Action Priority Matrix with P1–P4 quadrants and animated, hoverable dots per row
- Export to CSV or PNG for team working documents and slide decks
- Security-hardened: API key proxied server-side, response headers, request body limits, CSV-injection escaping, and no error disclosure

---

### Monocular Metric-Depth Validation Harness *(repository private)*

A reproducible harness that measures **where a learned monocular depth model stops being trustworthy** — capturing color frames on a tablet with no depth sensor at all, scoring predicted depth against a physically measured ground-truth plane, and contrasting the learned model's error against a first-principles Time-of-Flight noise model on one plot.

The finding it is built to show: a learned model and a physical depth sensor fail for different reasons. The sensor degrades from photon statistics (error linear in distance); the model degrades from missing visual cues (error that drifts and curves with range and texture). The deliverable is an operating envelope — *usable for AR placement beyond 1.5 m, not for sub-centimeter metrology* — stated as an engineering discipline, not a benchmark score.

**Stack:** Python · NumPy · Matplotlib · pandas · Depth Pro (Apple) · Depth Anything V2 (PyTorch / Hugging Face)

- Dense per-pixel ground truth from a measured plane — perpendicular for a single distance, rotated for a closed-form depth gradient
- Literature-standard metrics: AbsRel, RMSE, and δ < 1.25ⁿ thresholds, comparable to published model papers
- Least-squares scale-and-shift alignment for relative-depth models; metric models scored directly and labeled as such
- Stress axes for distance and surface texture, with documented ground-truth error budget and assumptions
- Runs end to end on synthetic data with no model weights and no photos, so the pipeline is unit-testable

---

### [ToF Depth Sensor Characterization Tool](https://github.com/seohoyoun-oss/tof-depth-sensor-characterization)

Python tool that simulates Time-of-Flight depth data with physics-based noise models and validates them against empirical statistics. Shot noise, ambient noise, residual-histogram validation, step-edge artifact scenes — the kind of analysis run on real hardware.

**Stack:** Python · NumPy · Matplotlib · LaTeX

- Poisson shot noise (σ grows linearly with distance), additive ambient Gaussian, RSS combination
- Annotated simulation-config diagram: 320 × 240 array, co-located VCSEL, tilted-plane scene from 0.3 m to 5.0 m
- Four output figures: depth map comparison, empirical vs. theoretical noise curves with the shot/ambient crossover marked, residual histograms at multiple distances, and a step-edge scene with flying-pixel boundary
- Companion physics study guide (PDF) deriving the noise models behind the simulation
- Configurable photon density spans low-cost consumer to industrial ToF regimes, with deterministic seeding for reproducible runs

---

### [Building a 6-inch Telescope by Hand](https://telescope-project.vercel.app) *(website)*

A personal site telling the story of grinding, figuring, and testing a 6-inch Newtonian reflector mirror by hand — from a raw Pyrex blank through ten months of grit, water, and shadow to first light — alongside a spec sheet of what the finished instrument actually measures. Designed at f/9; the mirror came out at f/9.5.

Plain HTML, CSS, and JavaScript — no framework and no build step, deployed as a static site.

**Stack:** HTML · CSS · JavaScript · Vercel

- Scroll-driven hero and reveal animations written by hand, with a six-frame gallery and a lightbox at full resolution
- Spec sheet reporting as-built values against design intent: 152 mm aperture, 1443 mm focal length, f/9.5, 0.91″ Rayleigh limit, ≈ 470× naked-eye light grasp
- Every photograph ships as AVIF with a JPEG fallback, generated with macOS `sips` — no image tooling in the pipeline
- Hardened deploy: strict CSP with a hash for the single inline script, HSTS, frame and MIME protections, and tuned cache lifetimes
- Split licensing — MIT for the code, all rights reserved for the photographs and prose, with third-party fonts and marks scoped separately
- Structured so sections on stars, planets, and the wider universe can be added later without a redesign

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/seoho-y-740506171)
