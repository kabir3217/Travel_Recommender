# Travel_Recommender
# 🌍 Travel Recommender Web App

This is a Flask-based Travel Recommender that helps users discover ideal travel destinations based on their preferences — including season, duration, budget, and interests. The app also generates a 7-day personalized itinerary for each city.

---

## 🚀 Features

- 🌤 Filter destinations by season, days, budget, and group size
- ❤️ Select personal interests like food, culture, adventure, nature, etc.
- 💡 Personalized 7-day itinerary generated dynamically
- 💰 See estimated total cost based on adults and children
- ⚡ Fast and simple interface with Flask + Jinja2
- 📄 Data loaded from structured CSV files

---

## 🗂️ Project Structure

```

travel-recommender/
├── app.py                  # Main Flask application
├── travel\_packages.csv     # List of destinations with price and rules
├── activities.csv          # Activities per city based on culture and interest
├── templates/
│   ├── index.html          # Home page with input form
│   └── results.html        # Output page with recommendations and itinerary
├── static/
│   └── images/             # Optional static images
└── README.md               # This file

````

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/travel-recommender.git
   cd travel-recommender
````

2. **Install required Python packages**

   ```bash
   pip install flask pandas
   ```

3. **Run the Flask app**

   ```bash
   python app.py
   ```

4. **Open in browser**

   ```
   http://127.0.0.1:5000/
   ```

---

## 📁 CSV Files

### `travel_packages.csv`

Contains 50–100 destinations with:

* `destination`, `season`, `min_days`, `max_days`, `min_people`, `max_people`, `price_per_adult`, `price_per_child`, `description`

### `activities.csv`

Each row represents one activity related to a destination:

* `destination`, `activity_no`, `activity_name`

Activities are curated by city culture, region, and travel theme (e.g., beaches in Goa, temples in Kyoto, art in Paris).

---

## ✅ Future Enhancements

* Add user login & save favorite trips
* Integrate Google Maps and live weather
* Let users drag and drop activities in itinerary
* Build a React frontend with a Flask API backend

---

## 🙋‍♂️ Author

**Kabir Singh**
Built with ❤️ using Python, Flask, and Pandas.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

```

