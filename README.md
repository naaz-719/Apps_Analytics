# Apps_Analytics

This project is a web-based dashboard that visualizes analytics for mobile apps. It provides insights into app ratings, reviews, installs, and categories using interactive charts built with Plotly.

- The dashboard is hosted live on GitHub Pages:
https://naaz-719.github.io/Apps_Analytics/

# Dashboard Features

# 1. Pie Chart: Install Distribution by Category

- Purpose: Shows the proportion of installs across different app categories.

- Implementation:

    - Uses Plotly Express px.pie.

    - Categories are colored with a pastel color palette.

    - Each slice includes hover-only insights (e.g., “Photography apps: highest installs”).

    - Black outline around slices for clarity (marker.line.color='black').

- Interactivity: Hovering over each slice displays additional information about that category.

# 2. Line Chart: Average Rating per Category

- Purpose: Displays trends in average ratings across app categories.

- Implementation:

      - Groups apps by category and calculates the mean rating.

      - Includes markers on each point for clarity (marker=dict(color='black')).

      - Hover-only insights show category-specific information.

- Filters: Can be adjusted to include only categories of interest (e.g., rating above a threshold).

# 3. Bar Chart: Total Review Count per Category

- Purpose: Shows the total number of user reviews per category.

- Implementation:

      - Bars are grouped by category.

      - Hover-only insights provide context (e.g., “High engagement”, “Moderate reviews”).

      - Colored using a pastel gradient for easy visual distinction.

- Interactivity: Hovering over a bar displays the total review count and a short insight.

# 4. Grouped Bar Chart: Average Rating vs Total Reviews

- Purpose: Compares average rating and total review count side by side for the top 10 app categories by installs.

- Implementation and filtering (from the code):

      - Includes only apps with average rating ≥ 4.0.

      - Only apps with size ≥ 10 MB are considered.

      - Only apps with last update in January are included.

      - Time-based conditional display:

      - This chart is only visible between 3 PM and 5 PM IST.

      - Outside this timeframe, the chart is hidden from the dashboard.

- Interactivity: Hovering over a bar shows a category-specific insight.

- Purpose of filter: Focuses the dashboard on high-quality apps during peak observation hours.

# Technical Details

- Built using Python and Plotly for interactive visualizations.

- Charts include hover-only insights for better user experience without cluttering the dashboard.

- The dashboard is fully static HTML and hosted via GitHub Pages, requiring no backend server.

- Colors and layouts are consistent across all charts for a clean, professional appearance.

# Usage Instructions

# Open the live dashboard: 
https://naaz-719.github.io/Apps_Analytics/

Hover over any chart element to see additional insights.

- For the grouped bar chart, note that it only appears between 3 PM and 5 PM IST.

# Future Enhancements

- Add real-time updates by fetching live app data from the Play Store.

- Include search or filter functionality for categories dynamically.

- Add downloadable CSV or Excel reports for each chart.

Include trend predictions using AI/ML for ratings or reviews.
