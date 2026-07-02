# Google Timeline Map Visualization

An interactive web-based map visualization tool for Google Timeline JSON data. Built with Leaflet.js, this tool transforms raw location history into an intuitive, color-coded journey map with detailed street-level logs.

## ✨ Features

- **Interactive Map** – Powered by Leaflet.js with multiple base layers (Google Streets, Satellite, Hybrid, and OpenStreetMap)
- **Color-Coded Paths** – Each route segment is colored by activity type (driving, walking, cycling, etc.)
- **Detailed Street Log** – Sidebar lists every segment with start/end times, coordinates, and point count
- **Date Filter** – Filter your timeline by specific dates
- **Activity Filter** – Show/hide specific activity types with checkbox controls
- **Segment Highlighting** – Click any log entry or map path to zoom in and highlight the route
- **Summary Dashboard** – View total distance, GPS points, segment count, and activity breakdown

## 🛠️ Technologies Used

- **Leaflet.js** – Interactive mapping library
- **Google Maps Tiles** – Base map layers (Streets, Satellite, Hybrid)
- **OpenStreetMap** – Fallback base layer
- **HTML/CSS/JavaScript** – Core frontend technologies

## 📁 File Structure

```
timeline-map/
├── index.html          # Main application file
└── timeline_data.js    # Timeline data (auto-generated)
```

## 🚀 Live Demo

**[View the live demo →](https://xiaoman0517.github.io/timeline-map/)**

## 📊 Data Format

The application expects a JavaScript array of segment objects with the following structure:

```javascript
const TIMELINE_DATA = [{
  startTime: "2026-03-29T13:37:00.000-04:00",
  endTime: "2026-03-29T13:37:00.000-04:00",
  points: [{ lat: 40.9138182, lng: -74.0638793, time: "..." }],
  activityType: "WALKING",  // or "IN_PASSENGER_VEHICLE", "CYCLING", etc.
  distanceMeters: 4553.36865234375
}];
```

## 🎨 Activity Color Reference

| Activity Type | Color |
|---------------|-------|
| Vehicle | Red (#e94560) |
| Walking | Green (#27ae60) |
| Cycling | Blue (#3498db) |
| Motorcycle | Orange (#e67e22) |
| Bus | Purple (#533483) |
| Train | Gold (#f39c12) |
| Unknown | Gray (#888888) |

## 🔧 How to Use

1. Clone or download this repository
2. Open `index.html` in your browser
3. The map will automatically load the timeline data
4. Use the filters in the sidebar to explore specific dates or activity types
5. Click on any route or log entry to highlight and zoom to that segment

## 📝 License

This project is available for demonstration and portfolio purposes.

---


---

