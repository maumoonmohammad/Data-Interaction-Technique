# Data Interaction Technique

An interactive data visualization web app, built with React, for exploring and comparing countries' economic and development indicators over time. The dataset covers GDP, GDP per capita, population, and HDI (Human Development Index) for countries from 1990 onward. The project demonstrates several data interaction and visualization techniques using different charting libraries.

## Visualizations

- **Scatter / bubble view (amCharts 5)** — An interactive XY chart with bubble and line series and a cursor, paired with a map-based navigator (continents rendered with a Natural Earth projection) for exploring the data.
- **Bar comparison (Plotly)** — A grouped bar chart that compares two selected countries for a chosen year, using dropdown selectors.
- **Line trends (Chart.js)** — A line chart that compares the GDP of up to three selected countries across the years.

## Interaction

Users pick countries and years from dropdown menus to update the charts, and navigate between the different chart views with React Router.

## Tech Stack

- **Framework:** React 18
- **Charting:** amCharts 5 (with geodata), Plotly.js, Chart.js (react-chartjs-2)
- **Routing:** React Router v6
- **Styling:** Bootstrap 5
- **Other:** React Helmet

## Getting Started

### Prerequisites
- Node.js

### Setup

```bash
# Clone the repository
git clone https://github.com/maumoonmohammad/Data-Interaction-Technique.git
cd Data-Interaction-Technique

# Install dependencies
npm install

# Start the development server
npm start
```

The app will open at `http://localhost:3000`.

To create a production build:

```bash
npm run build
```

## Project Structure

- `src/App.js` — amCharts 5 visualization with the XY chart and map navigator
- `src/barchart.js` — Plotly grouped bar chart comparing countries by year
- `src/line.js` — Chart.js line chart comparing countries' GDP over time
- `countries.js`, `new_countries.js` — the country indicator data
