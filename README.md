# Network Health Overview Dashboard 
This repository contains the setup for a **Network Health Overview Dashboard**, designed to provide real-time insights into crucial network performance indicators.


## Use Case: Detecting Underperforming Cell Sites 
This dashboard tackles the critical need for **detecting and monitoring** underperforming cell sites across various regions. By visualizing key network health KPIs, RF engineers can quickly identify anomalies, track trends, and drill down into site-level details to ensure optimal network performance.


## Objective
The primary objective of this project was to leverage **Palantir Foundry's** capabilities to build an interactive dashboard that enables network operations teams to:
* Monitor network health at a glance.
* Visualize anomalies and trends in real-time.
* Drill down into specific regional and site-level insights.


## Outcome 
A no-code, interactive dashboard tailored for network operations teams, providing a powerful tool for proactive network management and troubleshooting.


## Tools Used 
This network health dashboard is built entirely on Palantir Foundry, utilizing its powerful data integration and visualization components:

**1. Pipeline Builder**

In Pipeline Builder, the following steps were undertaken to prepare the data:
* **Data Ingestion:** Ingested a raw CSV file containing network data.
* **Data Transformation:** Split the ingested data into two distinct datasets: **site metadata and KPI logs.**
* **Data Cleaning & Joining:** Cleaned and joined these datasets based on ``Site ID`` and ``Date`` for comprehensive data linkage.
* **Metric Aggregation:** Aggregated key performance metrics to calculate site availability and other crucial KPIs (Call Drop Rate, Throughput) categorized by ``Region``.
* **Output Preparation**: Created final, refined datasets and object types optimized for UI consumption.



**2. Workshop Module**

The Workshop module was used to construct the interactive user interface, featuring:
* **Interactive Filters:** Implemented dynamic filters for Region, Technology, Supplier, and Site to allow granular data exploration.
* **Key Metric Cards:** Displayed prominent KPIs such as average throughput, call drop rate, units sold, revenue, and market share for quick overview.
* **Visualizations:**
  * **Charts:** Integrated charts showcasing revenue by region and KPI trends over time.
  * **Tables:** Provided detailed tables for inventory and health data.
  * **Geo Map:** A geographic map was included to visualize site availability by region, offering spatial insights into network health.
  * **Tabbed Navigation:** Organized all visualizations and data points into toggleable tabs for seamless navigation and anomaly monitoring.


## Installation Guide

#### Upload Package to Your Enrollment
The first step is to upload your project package to the Foundry Marketplace:
  * **Download:** Obtain the project's ``.zip file`` from this GitHub repository.
  * **Access Marketplace:** Navigate to your enrollment's marketplace at: ```{enrollment-url}/workspace/marketplace```
  * **Initiate Upload:** In the marketplace interface:
      * Select or create a store within your preferred project folder.
      * Click the "Upload to Store" button.
      * Choose your downloaded .zip file.
        
#### Install the Package
Once uploaded, you will need to install the package within your Foundry environment. For detailed, official instructions, please refer to the Palantir documentation.

The installation process typically involves four main stages:

1. **General Setup:**

    * Configure the desired package name.
    * Select the appropriate installation location.

2. **Input Configuration:**

    * Configure any required inputs. If no inputs are specified, you can proceed to the next step.
    * Consult the project documentation for specific input requirements.

3. **Content Review:**

    * Review the resources that will be installed, such as the Developer Console, the Ontology, and Functions.

4. **Validation:**

    * The system will perform checks for any configuration errors.
    * Resolve any flagged issues before proceeding with the installation.
    * Initiate the installation once validation is successful.
