# ✈️ Travel Planner CrewAI

A smart, interactive multi-agent system powered by [CrewAI](https://github.com/joaomdmoura/crewai) that helps travelers plan unforgettable trips!  
From flights to food, each AI agent plays a specialized role in crafting a **personalized, day-by-day itinerary**, delivered in Markdown format.

---

## 🧠 What It Does

Given user inputs such as:

- 📍 Destination
- 📅 Travel dates
- 💸 Budget
- ✨ Travel style / preferences

This autonomous AI crew collaboratively:

1. Finds optimal **flight options**
2. Recommends the best **accommodations**
3. Plans engaging **daily activities**
4. Curates delicious **local food spots**
5. Assembles everything into a **ready-to-use travel itinerary**

---

## 👥 The Crew

| Agent               | Role                            | Goal                                                                      |
|---------------------|----------------------------------|---------------------------------------------------------------------------|
| Flight Expert        | Flight Deal Hunter              | Find the most optimal flights for the given dates and budget.             |
| Accommodation Guru  | Stay Specialist                 | Suggest top-rated hotels or Airbnbs based on user preferences.            |
| Local Tour Curator   | Activity Designer               | Build a daily plan of attractions, tours, and experiences.                |
| Foodie Guide         | Culinary Consultant             | Recommend must-try dishes, restaurants, and local food gems.              |
| Itinerary Architect  | Journey Composer                | Combine all outputs into a seamless, beautiful travel plan.               |

Each agent can use specific **tools or APIs** (Skyscanner, Booking.com, Airbnb, etc.) to power their decisions.

---

## 🔧 Tech Stack

- [CrewAI](https://github.com/joaomdmoura/crewai) — Multi-agent orchestration
- `crewai_tools` — For web/API integrations
- External APIs (to be implemented):
  - ✈️ [Skyscanner](https://rapidapi.com/skyscanner/api/skyscanner-flight-search) or [Kiwi](https://docs.kiwi.com/)
  - 🏨 [Booking.com API](https://developers.booking.com/) or [Airbnb unofficial APIs]
  - 🍽️ Yelp or Google Maps for food recommendations

---
## 📂 Project Structure
travel_planner_ai/
├── README.md
├── pyproject.toml
├── src/
│   └── travel_planner/
│       ├── config/
│       │   ├── agents.yaml
│       │   └── tasks.yaml
│       ├── tools/
│       │   ├── flight_search_tool.py
│       │   ├── hotel_search_tool.py
│       │   └── food_search_tool.py
│       ├── crew.py
│       └── main.py

## 🧩 Features To Implement
- ✅ Sequential & interactive planning

- ⏳ Feedback loops (e.g., confirm flights before booking hotels)

- 📄 Exportable Markdown or PDF itineraries

- 🔌 Plug-and-play API tool integrations

- ✍️ Natural language input