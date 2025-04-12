# 🌍 AI Travel Planner

A multi-agent system for personalized, end-to-end travel planning powered by **Anthropic Claude** and a **Gradio web interface**.

---

## 🧠 Overview

This AI Travel Planner leverages **specialized AI agents**, each responsible for a distinct part of trip planning. Together, they deliver a comprehensive travel plan tailored to your preferences and constraints.

---

## ✨ Key Features

- **🗓️ Itinerary Generator** — Day-by-day travel schedule based on interests and trip duration  
- **🚆 Transportation Specialist** — Recommends optimal travel options to/from destination  
- **🏨 Accommodation Finder** — Suggests hotels or stays based on your budget and needs  
- **📍 Local Information Expert** — Provides cultural tips, weather, safety, and events  
- **💸 Budget Analyzer** — Helps optimize spending with smart, cost-saving strategies  

---

## ⚙️ How It Works

1. **📝 Input Collection**  
   - Users provide basic details (origin, destination, dates, preferences)

2. **🧩 Agent Orchestration**  
   - Claude-powered agents process your input sequentially for each travel aspect

3. **📤 Comprehensive Output**  
   - Returns a full travel plan covering itinerary, logistics, budgeting, and local info

---

## 🛠️ Installation

### 🔧 Prerequisites

- Python 3.8+
- Anthropic API key

### 📦 Setup

```bash
# Clone the repo
git clone https://github.com/Vishwajeet0830/TravelMultiModalAgent.git
cd TravelMultiModalAgent

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install anthropic gradio streamlit pydantic

# Store your API key
echo "ANTHROPIC_API_KEY=your_api_key_here" > .env
