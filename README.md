<h1> Population Migration & Political Realignment (2020–2024)</h1>

<p>
This project examines how <b>post-Covid population migration</b> relates to changes in <b>partisan voting</b> between the 2020 and 2024 U.S. presidential elections. 
By combining county- and state-level demographic data with election results, the analysis explores whether areas with faster population growth also tended to shift more Republican in 2024.
</p>

<h2>Objectives</h2>
<ul>
  <li>Measure <b>population density change</b> (2020→2024) at county and state levels.</li>
  <li>Quantify <b>Republican vote share change</b> (2020→2024).</li>
  <li>Assess the <b>correlation</b> between population migration and partisan outcomes.</li>
  <li>Visualize geographic patterns with interactive <b>Folium choropleths</b> and <b>scatterplots</b>.</li>
</ul>

<h2>Data Sources</h2>
<ul>
  <li><a href="https://www.census.gov/data/datasets/time-series/demo/popest/2020s-counties-total.html"><b>U.S. Census Bureau County Population Totals</b></a> — track population inflows/outflows (2020–2024).</li>
  <li><a href="https://data.census.gov/table?q=GEOINFO&g=010XX00US$0500000&d=GEO+Geography+Information"><b>U.S. Census Bureau GEOINFO (Geography Information)</b></a> — county <b>land area</b> used to compute density.</li>
  <li><a href="https://www.ers.usda.gov/data-products/rural-urban-continuum-codes"><b>USDA Rural–Urban Continuum Codes</b></a> — classify metro vs. non-metro counties.</li>
  <li><a href="https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/VOQCHQ"><b>MIT Election Data & Science Lab</b></a> — county presidential returns (2020 & 2024).</li>
</ul>

<h2>Key Analyses & Findings</h2>
<ul>
  <li><b>Population Density Mapping:</b> County-level maps (green = increase, red = decrease) highlight growth pockets across key regions.</li>
  <li><b>Partisan Shift Mapping:</b> County-level maps (red = GOP gain, blue = Dem gain) show widespread Republican improvements across swing states.</li>
  <li><b>Correlation (County, Population-Weighted):</b> In counties that increased GOP share, density growth shows a modest positive association (r ≈ +0.26); in counties that decreased GOP share, the association is moderately negative (r ≈ −0.33). Larger counties carry more influence.</li>
  <li><b>Correlation (State Level):</b> Across swing states, <b>population density growth correlates positively</b> with increased Republican vote share (<b>r = 0.51</b>), suggesting migration and population expansion likely played a meaningful role in 2024 outcomes.</li>
</ul>

<h2>Swing State Highlights</h2>
<table>
  <thead>
    <tr>
      <th>State</th>
      <th>Δ Population Density (2020→2024)</th>
      <th>Δ GOP Vote Share (p.p.)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><b>Arizona</b></td><td>+5.93%</td><td>+4.38</td></tr>
    <tr><td><b>Georgia</b></td><td>+4.36%</td><td>+1.45</td></tr>
    <tr><td><b>North Carolina</b></td><td>+5.79%</td><td>+1.25</td></tr>
    <tr><td><b>Nevada</b></td><td>+5.21%</td><td>+1.13</td></tr>
    <tr><td><b>Wisconsin</b></td><td>+1.13%</td><td>+1.20</td></tr>
    <tr><td><b>Michigan</b></td><td>+0.61%</td><td>+1.18</td></tr>
    <tr><td><b>Pennsylvania</b></td><td>+0.58%</td><td>+0.86</td></tr>
  </tbody>
</table>

<h2>Tools</h2>
<ul>
  <li><b>Python:</b> pandas, numpy, matplotlib, seaborn, folium</li>
  <li><b>Jupyter / CyberGISX</b> for analysis and notebooks</li>
  <li><b>GeoJSON & Folium</b> for interactive mapping</li>
</ul>

<h2>Reproducing the Maps</h2>
<ul>
  <li>If notebook trust is restricted, each map cell saves an interactive HTML:
    <code>m_density.save("swing_states_density_change.html")</code> and
    <code>m_vote.save("swing_states_vote_shift.html")</code>.
  </li>
  <li>Open directly in a browser (works without notebook trust):
    <code>webbrowser.open("swing_states_density_change.html")</code>.
  </li>
</ul>

<h2>Key Takeaway</h2>
<p>
Post-pandemic migration reshaped not only where Americans live but also how they vote. 
Growth in larger, fast-expanding counties aligns with <b>Republican gains</b> in 2024, indicating that demographic mobility and political change moved together in meaningful ways.
</p>
