# AI Travel Planner

A multi-agent AI system for comprehensive travel planning built with Anthropic Claude and Gradio.

## Overview

This AI Travel Planner uses multiple specialized AI agents to create personalized travel plans. Each agent focuses on a specific aspect of trip planning, collaborating to provide a comprehensive travel experience tailored to your preferences.


## Features

- **Itinerary Generator**: Creates day-by-day travel plans customized to your preferences
- **Transportation Specialist**: Suggests optimal ways to reach your destination
- **Accommodation Finder**: Recommends places to stay based on your requirements
- **Local Information Expert**: Provides essential details about your destination
- **Budget Analyzer**: Optimizes your travel budget and offers money-saving tips

## How It Works

The system utilizes a multi-agent architecture where each agent is powered by Anthropic's Claude AI:

1. **Input Collection**: Users provide basic travel details (departure location, destination, travel dates, etc.)
2. **Agent Orchestration**: Each specialized agent processes the information sequentially
3. **Comprehensive Output**: The system generates detailed travel recommendations across multiple categories

## Installation

### Prerequisites
- Python 3.8+
- An Anthropic API key

### Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-travel-planner.git
cd ai-travel-planner
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install anthropic gradio streamlit pydantic
```

4. Set up your API key:
```bash
# Create a .env file with your API key
echo "ANTHROPIC_API_KEY=your_api_key_here" > .env
```

## Usage

### Local Deployment

Run the application with Gradio:

```bash
python gradio_app.py
```

This will launch a web interface where you can:
1. Enter your travel details (origin, destination, dates, etc.)
2. Click "Plan My Trip" to generate your personalized travel plan
3. View the results organized in tabs (Itinerary, Transportation, Accommodation, Local Info, Budget)

### Google Colab Deployment

You can also run this project in Google Colab:

1. Upload the `travel_planner.py` and `gradio_app.py` files to your Colab environment
2. Store your Anthropic API key in Colab's secrets manager
3. Run the application with:
```python
!python gradio_app.py "$ANTHROPIC_API_KEY"
```

## Project Structure

- `travel_planner.py`: Contains the multi-agent implementation with specialized travel planning functions
- `gradio_app.py`: Implements the web interface using Gradio

## Agent Descriptions

1. **Itinerary Planner Agent**
   - Creates a detailed day-by-day itinerary
   - Considers trip duration, traveler preferences, and budget

2. **Transportation Agent**
   - Suggests optimal transportation options
   - Provides cost estimates, travel times, and pros/cons

3. **Accommodation Agent**
   - Recommends lodging options at different price points
   - Includes location benefits and amenities

4. **Local Information Agent**
   - Provides weather forecasts, cultural tips, and safety information
   - Highlights special events and local transportation options

5. **Budget Analysis Agent**
   - Optimizes budget allocation across different categories
   - Offers destination-specific money-saving tips

## Future Enhancements

- **Real-time Data Integration**: Incorporate live flight and hotel pricing
- **Interactive Itinerary Editing**: Allow users to modify and refine generated plans
- **Map Visualization**: Add visual mapping of recommended activities
- **Travel Booking**: Add direct booking capabilities for flights and accommodations
- **User Accounts**: Save and manage multiple trip plans

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


## Acknowledgments

- Anthropic for the Claude API
- Gradio team for the web interface library
- All contributors to this project
