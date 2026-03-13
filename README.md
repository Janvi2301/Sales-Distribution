<h1 align="center">📊 Sales Distribution Dashboard</h1>

<p align="center">
An interactive Power BI dashboard designed to analyze sales performance across regions, products, and customers.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Power%20BI-yellow">
  <img src="https://img.shields.io/badge/Data-CSV-blue">
  <img src="https://img.shields.io/badge/Language-DAX-green">
  <img src="https://img.shields.io/badge/Domain-Data%20Analytics-orange">
</p>

---

<h2>📌 Short Description</h2>

<p>
The Sales Distribution Dashboard is an interactive Power BI project designed to analyze sales performance across different regions, products, and customers. The dashboard provides insights into total sales, regional distribution, product performance, and monthly sales trends through intuitive visualizations. A unique feature of this dashboard is the dynamic theme switcher, allowing users to toggle between dark mode and light mode, improving usability and enhancing the visual experience.
</p>

---

<h2>🎯 Goal of the Dashboard</h2>

<p>
The goal of this dashboard is to transform raw sales data into meaningful insights that help identify top-performing regions, products, and customers. By combining interactive filters and clear visualizations, the dashboard enables users to explore sales patterns, compare actual sales with targets, and understand overall business performance more effectively.
</p>

---

<h2>🛠 Tech Stack</h2>

<ul>
<li>📊 <b>Power BI Desktop</b> – Used to build a creative and interactive sales dashboard with custom visuals, filters, and dynamic theme functionality.</li>
<li>🔄 <b>Power Query</b> – Used for data cleaning, transformation, and preparing datasets for analysis.</li>
<li>🧠 <b>DAX (Data Analysis Expressions)</b> – Used to create measures for key metrics and conditional formatting to support dynamic dashboard behavior.</li>
</ul>

---

<h2>📂 Data Source</h2>

<p>
The dataset used in this project is a CSV file containing sales-related information such as products, regions, customers, and sales values used to analyze overall business performance.
</p>

---

<h3>🌗 Dynamic Theme Switching (Dark / Light Mode)</h3>

<p>
This dashboard includes a dynamic theme toggle that allows users to switch between 
<b>Dark Mode</b> and <b>Light Mode</b> for a better viewing experience. A dedicated 
<b>Theme table</b> was created containing a value used to control the dashboard theme.
</p>

<p>
Using a DAX conditional expression, visual colors are dynamically updated across the 
entire dashboard based on the selected theme.
</p>

<pre>
Theme Color = IF(SUM(Theme[Value]) = 1, "Dark Color", "Light Color")
</pre>

<p>
The measure is applied to visual elements such as backgrounds, fonts, and chart colors 
through Power BI’s <b>Conditional Formatting → Format by Field Value</b> option, allowing 
all visuals to automatically update when the theme button is toggled.
</p>

<p>
This feature improves dashboard usability and demonstrates the use of 
<b>DAX-driven conditional formatting</b> to create a more interactive user interface.
</p>

---

<h2>Walkthrough of Key Visual</h2>

<ul>

<li><b>Region-wise Sales Distribution (Donut Chart)</b> – Displays the proportion of total sales contributed by each region, helping identify the regions generating the highest revenue.</li>

<li><b>Global Sales Map</b> – Visualizes sales distribution across different locations on the map to provide a geographic perspective of business performance.</li>

<li><b>Product vs Sales (Bar Chart)</b> – Compares sales across different products to identify top-performing and low-performing products.</li>

<li><b>Monthly Sales vs Target (Column Chart)</b> – Shows the comparison between actual sales and target sales for each month to evaluate performance against business goals.</li>

<li><b>Weekly Sales Trend (Line Chart)</b> – Illustrates sales patterns across weeks to track fluctuations and identify trends over time.</li>

<li><b>Product & Region Performance Filter (Slicer)</b> – An interactive slicer that allows users to filter and analyze sales performance by product across different regions, weeks, and months.</li>

</ul>

---
