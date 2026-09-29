# Audio Media Maturity Diagnostic Tool

An interactive, single-page web diagnostic instrument calibrated for the audio media industry (radio, podcasting, and digital streaming). The tool evaluates an organization's digital capabilities across five core dimensions to compute maturity scores, classify the organization into a strategic profile, and provide tailored AI-driven strategic guidance.

---

## What It Does

- **5-Dimension Capability Assessment**: Evaluates organizations across 15 observable, leveled indicators (Stages 1–5):
  - **Listener Data Infrastructure**: Data matching, quality monitoring, and governance.
  - **Listening & Engagement Channels**: Device availability, listening continuity, and feedback loops.
  - **Content & Ad Operations Automation**: Workflow automation, delivery reporting, and error handling.
  - **AI-Driven Personalization & Monetization**: Recommendation systems, model deployment, and performance validation.
  - **Audio Media Change Capacity**: Cross-functional ownership, adoption management, and iterative learning.
- **Scoring & Archetype Profiling**: Calculates dimension scores and an unweighted overall score (1.0–5.0), mapping results to strategic archetypes such as *Still On the Air*, *Category Leader*, *Flying Blind*, *The Execution Gap*, *Everywhere but Generic*, or *Mixed Pattern*.
- **Interactive Visualizations**: Renders dynamic radar and horizontal bar charts using Chart.js. Clicking any axis point or bar navigates directly to the corresponding dimension breakdown.
- **AI-Powered Diagnostics** *(Requires API Key)*:
  - **Strategic Sub-Profiling**: Generates an enhanced evaluation highlighting organizational strengths and blind spots.
  - **Interactive AI Consultant**: A conversational assistant pre-prompted with your specific assessment scores and answers.
  - **Adaptive AI Deep Dive**: Identifies your lowest-scoring dimension and dynamically creates leveled follow-up diagnostic questions in real time, updating your maturity score live.
  - **Multi-Model Fallback & Racing**: Concurrently queries Google Gemini and OpenAI endpoints to select the fastest streaming response.

---

## How to Use the Webpage

### 1. Opening the Tool
The tool is a self-contained HTML page that requires no server, build tools, or dependencies. 
- Open `group9_week5_partc.html` directly in any modern web browser (Chrome, Edge, Firefox, Safari).

### 2. (Optional) Configuring API Keys
To enable AI features, navigate to the **API Settings** tab at the top right before or during your assessment:
1. Enter a **Google Gemini API Key** (primary) and/or an **OpenAI API Key** (optional fallback).
2. Once a valid key is detected, the **AI Features** toggle in the navigation bar automatically activates.
> *Note: API keys are stored in browser memory only and communicate directly with Google and OpenAI endpoints. They are never transmitted to external servers.*

### 3. Completing the Assessment
1. Enter your organization or business unit name.
2. Step through each of the 5 dimensions, selecting the stage description that best reflects your current operational reality over the past 12 months.
3. Click **Next** to move between dimensions, or use **Skip to Results (Test)** to populate sample data quickly for demonstration.
4. Click **Calculate Maturity Score** on the final step.

### 4. Exploring Diagnostic Results
- **Overall Score Card & Archetype**: Review your aggregate stage score and read the strategic recommendation for your profile.
- **Radar & Bar Charts**: Inspect your capability distribution visually. Click on any chart element to jump to that dimension's detailed response history.
- **AI Deep Dive**: If AI features are active, click **Start AI Deep Dive** to generate granular diagnostic questions targeting your lowest-scoring capability area.
- **AI Consultant**: Scroll to the bottom of the results page to chat directly with the AI consultant about your specific bottlenecks and implementation roadmaps.

---

## How to Obtain Required API Keys

### Google Gemini API Key (Recommended / Primary)
1. Visit [Google AI Studio](https://aistudio.google.com/).
2. Sign in with your Google account.
3. In the left navigation menu, click **Get API key**.
4. Click **Create API key** (select an existing Google Cloud project or generate a new one).
5. Copy the generated key and paste it into the **Google Gemini API Key** field in the tool's **API Settings** tab.

### OpenAI API Key (Optional / Fallback)
1. Visit the [OpenAI Platform](https://platform.openai.com/).
2. Log in or create an account.
3. Navigate to **API Keys** under the **Dashboard** (or go directly to [platform.openai.com/api-keys](https://platform.openai.com/api-keys)).
4. Click **Create new secret key**, give it an optional label, and copy the secret key.
5. Paste it into the **OpenAI API Key** field in the tool's **API Settings** tab.

---

## Technologies Used

- **Tailwind CSS (CDN)**: Layout styling and typography.
- **Chart.js**: Interactive radar and bar chart visualizations.
- **Marked.js**: Real-time Markdown rendering for AI responses.
- **Google Generative Language API & OpenAI Chat Completions API**: Server-sent event (SSE) streaming for AI insights.

---

## Project Team (Group 9)

- Giang Khuu
- Lira Sandoval Campos
- Hudson Trussell
- Azimjon Izzatillaev