---
datapackage:
  title: Cabo Verde Startup Database
  description: Datas
  created: 2024-07-09
  updated: 2024-07-12
  sources:
  - path: https://airtable.com/appGsydkfn1oLYQco/shrEqU9DbVFhVhhl7/tblKkPhhqZg8ROraG
    title: Link to data source
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - name: cabo-verde-startup-databse
    title: Cabo Verde - Startup Database
    description: The "Cabo Verde Startup Database" is a detailed CSV file that showcases the startup ecosystem in Cabo Verde. It includes essential information about various startups, such as their names, headquarters locations, core business areas, websites, descriptions, business models, stages/types, and the powering entity (CVD). This database offers a concise snapshot of the innovative ventures across Cabo Verde's islands, making it a valuable resource for networking, research, and support. 
    lastModified: 2024-07-12
    path: ./data/cabo-verde-startup-databse.csv

---

# Cabo Verde Startup Database Visualizations

## Number of Startups by Island

<PlotlyBarChart
  data={{
    url: 'https://raw.githubusercontent.com/AlvaroLima/cabo-verde-datahub/main/data-catalog/data/cabo-verde-startup-database.csv'
  }}
  title="Number of Startups by Island"
  xAxis="Localização HQ (Ilha)"
  yAxis="ID"
/>

## Percentage Distribution of Startups by Core Business

<PlotlyBarChart
  data={{
    url: 'https://raw.githubusercontent.com/AlvaroLima/cabo-verde-datahub/main/data-catalog/data/cabo-verde-startup-database.csv'
  }}
  title="Percentage Distribution of Startups by Core Business"
  xAxis="Core Business"
  yAxis="ID"
/>