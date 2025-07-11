# PageRank Calculator Web Application

A web application to calculate PageRank for websites using Google's PageRank algorithm.

## Getting Started

### Requirements
- Python 3.7+
- Node.js 14+
- npm or yarn

### Step 1: Backend Setup (Python/Flask)

1. **Create a Python virtual environment:**
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

2. **Install dependencies:**
```bash
pip install -r requirements.txt
```

3. **Run the backend server:**
```bash
python app.py
```

The backend will run at: `http://localhost:5000`

### Step 2: Frontend Setup (React)

1. **Navigate to the frontend directory:**
```bash
cd frontend
```

2. **Install dependencies:**
```bash
npm install
```

3. **Run the frontend development server:**
```bash
npm start
```

The frontend will run at: `http://localhost:3000`

### Step 3: Using the Application

1. Open your browser and go to: `http://localhost:3000`
2. Enter the URLs to analyze (one per line)
3. Click "Calculate PageRank"
4. View the results and chart

## Project Structure

```
PageRank_Web/
├── app.py                 # Backend Flask server
├── requirements.txt       # Python dependencies
├── frontend/              # React frontend
│   ├── src/
│   │   ├── App.js        # Main React component
│   │   ├── App.css       # Styles
│   │   └── logo.svg      # Logo
│   ├── package.json      # Node.js dependencies
│   └── public/
└── README.md
```

## Features

- **PageRank Calculation:** Uses Google's PageRank algorithm
- **Modern UI:** Clean blue and white design
- **Visualization:** Results displayed as a table and bar chart
- **Responsive:** Works on both mobile and desktop
- **Real-time:** Instant calculation and display

## Troubleshooting

### Common Issues:

1. **Port 5000 already in use:**
```bash
# Change port in app.py
app.run(debug=True, port=5001)
```

2. **Port 3000 already in use:**
```bash
# React will prompt to use another port
# Or stop the process using port 3000
```

3. **CORS Error:**
- Ensure the backend is running
- Check the API URL in the frontend

4. **Dependency Errors:**
```bash
# Backend
pip install --upgrade pip
pip install -r requirements.txt

# Frontend
npm install --force
```

## How to Use

1. **Enter URLs:** One per line
   ```
   https://example.com
   https://example.org
   https://example.net
   ```

2. **Calculate:** Click "Calculate PageRank"

3. **Results:**
   - PageRank ranking table
   - Visualization chart
   - Scores from 0-1 (higher = more important)

## PageRank Algorithm

PageRank calculates the importance of a web page based on:
- The number of links to the page
- The importance of linking pages
- Damping factor (usually 0.85)

Formula: `PR(A) = (1-d)/N + d∑PR(Ti)/C(Ti)`

## Notes

- Ensure both backend and frontend are running
- URLs must include protocol (http:// or https://)
- Some websites may block crawlers
- Results depend on the link structure between pages

## UI Design

- **Colors:** Blue and white (#2196F3,#1976D2)
- **Logo:** Math-inspired with PageRank formula
- **Responsive:** Works on all devices
- **Animations:** Smooth transitions

### Final Links

*   **Backend:** `https://final-web-pagerank.onrender.com`
*   **Frontend:** `https://finalwebpagerank.netlify.app` 