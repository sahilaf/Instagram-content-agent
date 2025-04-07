# 📱 Instagram Content Strategy CrewAI Project

An intelligent automation system built with **CrewAI** to streamline your **Instagram content strategy** — from market research and planning to visual concept creation and copywriting.


## 🧠 Overview

This project automates the creation of a powerful content strategy tailored to your Instagram niche and weekly focus areas. Using CrewAI, it brings together multiple specialized agents to:
- Research trends
- Build content calendars
- Design visual concepts
- Write compelling captions


## 🚀 Key Features

- **🔍 Automated Market Research**  
  Scrapes Instagram and web data to identify:
  - Trending topics
  - Relevant hashtags
  - Competitor strategies

- **📅 Weekly Content Calendar**  
  Develops a strategic plan with daily post ideas and themes.

- **🎨 Visual Concept Creation**  
  Produces image descriptions to guide AI image generation tools.

- **✍️ SEO-Optimized Copywriting**  
  Writes attention-grabbing captions with relevant hashtags and CTAs.

- **📄 End-to-End Strategy Report**  
  Generates a comprehensive `report.md` with all content assets for the week.

---

## ⚙️ How It Works

Each AI agent in the Crew has a dedicated role:

| Agent | Role |
|-------|------|
| **Market Research Agent** | Analyzes trends and competitors using search tools |
| **Content Strategist Agent** | Builds a content calendar using research insights |
| **Visual Creator Agent** | Describes visual content for each post |
| **Copywriter Agent** | Writes engaging and optimized captions |
| **Report Generator** | Compiles a full content strategy report |

---

## 📦 Installation

> **Python version required:** `>=3.10 <=3.13`  
> **Dependency manager:** [Poetry](https://python-poetry.org/)

### Step 1: Install Poetry (if not installed)
```bash
pip install poetry
```
### Step 2: Clone this repository and navigate into it
```bash
cd instagram-content-agent
```
### Step 3: Install dependencies
```bash
poetry lock
poetry install
```

### 🔧 Customization
1. Add Your API Key
Create a .env file in the root directory:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

2. Configure Your Agents
Edit src/instagram/config/agents.yaml to define agent roles, tools, and personalities.

3. Define Tasks
Edit src/instagram/config/tasks.yaml to assign objectives to each agent.

4. Customize Core Logic
Modify these files for more advanced configurations:

src/instagram/crew.py: Logic, tools, and argument setup

src/instagram/main.py: Customize user inputs and execution

### ▶️ Running the Project
From the root folder, start the crew and generate your content strategy:

```bash

poetry run instagram
```
This command will trigger all agents to:

Perform research

Develop content

Generate a complete report.md file in the root directory

### 🧬 Understanding the Crew Structure
Agents → Defined in config/agents.yaml

Tasks → Defined in config/tasks.yaml

Execution Logic → Controlled in crew.py and main.py

All agents collaborate to deliver a seamless content strategy pipeline.

### 📄 License
This project is licensed under the MIT License.
See the LICENSE file for full details.
