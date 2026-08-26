# NCRB Crime Data Dashboard: 2023 Analysis

A public-facing analytical dashboard visualizing 2023 rape case data from the National Crime Records Bureau (NCRB) of India. 

The goal of this project was to take a complex, raw government dataset (provided in CSV format) and translate it into a clean, easy-to-read web interface. The primary focus was on **UI/UX planning and responsible data visualization**—presenting sensitive statistics with clear context and a strong visual hierarchy.

## Design & Development Approach

Rather than relying on heavy charting libraries, I planned and built this dashboard using plain HTML, CSS, and JavaScript. This kept the project lightweight and allowed me to focus on how the information is structured.

* **Visualizing Data with CSS:** Instead of importing external libraries, I built simple, custom horizontal bar charts using CSS gradients and percentage widths controlled by JavaScript.
* **Information Layout:** I segmented the data into digestible panels (Key Insights, Geographical Distribution, Circumstances) to guide the user's reading flow without overwhelming them with raw numbers.
* **Responsive Design:** Used CSS Grid and Flexbox layouts to ensure the data remains legible and well-structured across desktop, tablet, and mobile devices.
* **Interactive Elements:** Added a simple JavaScript toggle to expand/collapse the full state rankings, keeping the initial view clean and focused on top-level insights.

## Data Source & Methodology

* **Source:** National Crime Records Bureau (NCRB) - Crime in India 2023 (Table 3A.11.0).
* **Data Integration:** The raw data was parsed and structured into JavaScript arrays and objects to render the charts and lists directly in the browser.

### Analytical Transparency
A critical part of planning this project was integrating a **Methodology** section directly into the UI. When dealing with crime data, it is essential to communicate caveats to the user. The dashboard explicitly clarifies:
1. **Reporting vs. Prevalence:** The numbers represent *registered* cases with authorities, not the total occurrence of sexual violence.
2. **Non-Additive Categories:** Circumstantial categories (e.g., Gang Rape, Custodial, Minors) are presented as separate data points so users do not inaccurately sum overlapping categories.
3. **Aggregate Exclusion:** "Total All India" and "Total State" rows from the raw CSV were filtered out of the state-level rankings to maintain data accuracy.

## Technical Stack
* **Structure:** HTML5
* **Styling:** CSS3 (Grid, Flexbox, Gradients, Media Queries)
* **Logic:** Vanilla JavaScript (Array mapping, simple DOM updates)

## How to Run

This is a static web page with no dependencies or installation required.
1. Clone or download the repository.
2. Navigate to the `rape_crime_dashboard` directory.
3. Open `index.html` in any modern web browser.