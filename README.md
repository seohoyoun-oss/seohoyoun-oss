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
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
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

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/seoho-y-740506171)
