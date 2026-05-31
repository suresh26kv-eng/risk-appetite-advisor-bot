# Conversational AI Risk Appetite Advisor

An interactive, browser-based financial technology application that utilizes generative AI to assess an investor's risk tolerance and provide structured, behavioral-finance-aligned asset allocation guidance. The system integrates Google's Gemini API with a dynamic Python UI deployment engine to simulate client advisory onboarding.

---

## Core Capabilities

### 1. Dynamic Advisory Interface
* Implements a stateful chat interface built on the Panel web app framework, rendering components natively inside computational notebooks or stand-alone browser servers.
* Features custom asynchronously bound triggers to collect user inputs, handle request latency with visual loading indicators, and update conversation threads dynamically.

### 2. Custom Prompt Engineering and Logic Partitioning
* Anchors a highly tailored background context array that enforces compliance-friendly behavioral parameters for investment assistants.
* Segregates financial personas into distinct risk archetypes:
  * **Low Risk:** Prioritizes capital preservation, advising low-volatility fixed-income instruments like government securities or fixed deposits.
  * **Medium Risk:** Recommends balanced index exposures and blue-chip equities coupled with risk-mitigating fixed-income allocations.
  * **High Risk:** Directs toward small-cap and growth equity categories, explicitly emphasizing capital compounding mechanics and volatility endurance.

### 3. API Adapter Architecture
* Formulates a specialized transformation layout wrapper to parse standardized conversational schemas into the specific nested layout parameters expected by the Gemini REST endpoints.
* Embeds structured configurations (including precise temperature modulation) to guarantee deterministic, focused, and compliance-appropriate dialogue delivery.

---

## Repository Structure

* **`Risk_Explaining_Bot.ipynb`**: The master file housing the back-end API infrastructure, prompt configuration matrix, layout bindings, and deployment-ready Panel dashboard canvas.

---

## Quantitative Stack & Requirements

The toolkit utilizes standard conversational AI and visualization frameworks:
* **requests:** Manages secure HTTP POST transactions directly with the Gemini v1beta gateway.
* **panel:** Builds responsive dashboard structures and handles style sheets for data presentation.

---

## How to Deploy and Run

### Prerequisites
Install the required application stack in your local python environment:
```bash
pip install requests panel jupyter
