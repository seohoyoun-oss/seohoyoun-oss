# Hi 👋, I'm Seoho

**Engineer who writes the tools that turn complex systems into decisions.**

Systems validation and optical engineer. I build Python tools to model sensors based on physics, and full-stack applications that bring AI into hardware program management workflows.

---

## Software Tools

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic_API-CC785C?style=for-the-badge&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
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

Built around a real-world pain point: issues surface without warning, teams scramble, and alignment breaks down. This tool makes the impact visible instantly and gives the program manager a structured, AI-assisted process to recover. Demo scenario is an 18-month robot vacuum launch spanning concept through EVT/DVT/PVT to mass production.

**Stack:** Next.js 16 · TypeScript · Tailwind CSS · Zustand + Immer · Framer Motion · Custom SVG Gantt · Anthropic API (Claude Sonnet) · Vercel

- Custom SVG Gantt with drag-to-move/resize bars, snapping to hardware-style B/M/E (1st/11th/21st) date boundaries
- Live risk scoring per task plus a program health dashboard (confidence, max slip, critical/at-risk/on-track counts)
- AI-identified affected tasks on issue entry, with hover preview of the full schedule impact before applying
- AI Risk Navigator: three mitigation options with trade-offs and a recommended path, committable in one click
- On-demand AI schedule audit covering risk blind spots, owner conflicts, and schedule compression
- Export to 8 formats: PNG, SVG, PDF, CSV, XLSX, and MS Project (MSPDI XML, MPP, MPX)

---

### [AI-Powered FMEA Assistant](https://github.com/seohoyoun-oss/epm-tool-fmea) · [Live Demo](https://epm-tool-fmea-qkrh.vercel.app)

A full-stack web application that accelerates Failure Mode and Effects Analysis for hardware program managers. Enter a design change description; the tool generates a structured FMEA table, ranks rows by Risk Priority Number, and plots them on an Action Priority Matrix mapping risk against implementation cost.

Built after running FMEA reviews on depth-sensing modules — the bottleneck on quality was always PM experience. The goal: compress that experience gap with a language model.

**Stack:** React 18 · Vite · Tailwind CSS · Anthropic API (Claude Sonnet) · Vercel serverless · PapaParse · html2canvas

- Generates 12–20 FMEA rows scoped to the stated design change (not a generic system survey)
- Editable table with live RPN recalculation; rows sortable and removable
- Action Priority Matrix with animated, hoverable dots per row
- Export to CSV or PNG for team working documents and slide decks
- API key never reaches the browser — proxied through a Vercel serverless function

---

### [ToF Depth Sensor Characterization Tool](https://github.com/seohoyoun-oss/tof-depth-sensor-characterization)

Python tool that simulates Time-of-Flight depth data with physics-based noise models and validates them against empirical statistics. Shot noise, ambient noise, residual-histogram validation, step-edge artifact scenes — the kind of analysis run on real hardware.

**Stack:** Python · NumPy · Matplotlib

- Poisson shot noise (σ grows linearly with distance), additive ambient Gaussian, RSS combination
- Four output figures: depth map comparison, empirical vs. theoretical noise curves, residual histograms at multiple distances, step-edge scene with flying-pixel boundary
- Configurable photon density spans low-cost consumer to industrial ToF regimes
- Deterministic output (`np.random.seed`) for reproducible characterization runs

---

### Design of Experiments Planning Assistant *(in development)*

Streamlit app that walks a hardware engineer from factor entry through fractional-factorial design generation, measurement upload, OLS regression fit, and main-effect plots — compressing hours of error-prone spreadsheet DOE setup into minutes. Repository goes public with the v0.1 deployment.

**Stack:** Python 3.11 · Streamlit · pyDOE2 · statsmodels · pandas · Matplotlib

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/seoho-y-740506171)
