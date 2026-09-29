# Audio Media Maturity Diagnostic Tool

An interactive, browser-based digital maturity benchmarking tool calibrated specifically for the audio media industry (radio broadcasters, streaming platforms, and podcast networks). 

The application evaluates an organization across 5 core capability dimensions, computes strategic archetypes, dynamically visualizes maturity profiles using Chart.js, and provides an optional client-side AI consultant for customized gap analysis and deep-dive question generation.

---

## Features

- **Company-Specific Benchmarking:** Input an organization name to personalize diagnostic profiles, score reports, and consultant analysis.
- **5 Diagnostic Capability Dimensions:**
  1. Listener Data Infrastructure (D1–D3)
  2. Listening & Engagement Channels (C1–C3)
  3. Content & Ad Operations Automation (O1–O3)
  4. AI-Driven Personalization & Monetization (A1–A3)
  5. Audio Media Change Capacity (G1–G3)
- **Overall Maturity Score:** Computes a composite score (1.00 to 5.00) that dynamically changes text color matching the 5 maturity stages (Magenta $\rightarrow$ Violet $\rightarrow$ Blue $\rightarrow$ Teal $\rightarrow$ Green).
- **Interactive Visualizations:** Capability Radar Chart and Score Breakdown Bar Chart rendered directly with Chart.js.
- **AI-Powered Diagnostics (Optional):**
  - **Strategic Sub-Profiles:** Model-generated operational analysis based on your exact answers.
  - **Dynamic Deep-Dive Questions:** Generates targeted diagnostic questions for your lowest-scoring capability areas.
  - **Interactive Consultant Chat:** Ask follow-up questions focused strictly on audio media operating maturity.

---

## Getting Started

This application is built as a single, self-contained HTML/JavaScript file with zero required build steps or local dependencies.

1. Clone or download this repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/<your-repo-name>.git
   cd <your-repo-name>