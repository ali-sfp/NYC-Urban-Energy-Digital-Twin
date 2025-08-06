This project explores rooftop solar potential across buildings in NYC’s ZIP code 10036 (Times Square / Midtown West), using openly available spatial data and solar radiation models.

The workflow integrates:

🛰️ PVGIS API — for solar irradiation estimates per rooftop
🐍 Python (GeoPandas, Requests, Shapely, TQDM) — for spatial processing and automation
🗺️ QGIS — for building footprint visualization and result mapping

🔄 Each building's centroid coordinates were sent to the PVGIS API to retrieve annual solar energy output per kW installed, assuming standard tilt and azimuth.
A sample of 998 buildings was used to comply with API rate limits.

✅ Results align with expected urban morphology:
High-rise buildings cast shadows, reducing solar exposure on adjacent rooftops — confirming the model reflects real-world spatial dynamics.

📈 Most rooftops receive between 1100–1400 kWh/year, with some exceeding 1450 kWh, indicating strong potential for distributed solar deployment.

⚙️ All outputs were saved as GeoJSON and CSV, ready for integration with spatial platforms.

🧠 This kind of workflow represents a foundational step toward creating urban-scale digital twins — combining geometry, physics, and environmental data to simulate city performance.
