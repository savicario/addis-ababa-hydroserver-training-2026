# HydroServer Training

**Workshop: Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems**

This repository contains the materials for the [HydroServer](https://hydroserver.org/) version 1.11 training to be held in Addis Ababa, Ethiopia, on September 14–17, 2026, as part of the Workshop *"Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems"* for the National Hydrological Services of Uganda, Rwanda, Ethiopia, and Kenya. TThe HydroServer training will take place on September 15, 2026, and will consist of four sessions.

Each country folder in this repository contains subfolders for the exercises. Each exercise folder includes the code and sample data needed to complete the exercise.


# Session 4a - Introduction to HydroServer: Architecture, Data Models & Deployment Options 

**Tuesday, September 15, 2026 | 09:00 – 10:40**

We will go through this [Presentation](https://www.canva.com/design/DAHTaIylsx4/UT70W8BzloZcVcoe-jTBig/edit) together. The presentation will provide an introduction to HydroServer, including what HydroServer is, its main components, the types of data and formats that can be managed through HydroServer, a brief overview of possible data ingestion options, and finally, the available deployment options. We will cover these topics in this order.


# Session 5a - Getting Started with HydroServer: Setup, Data Management, and Observations

**Tuesday, September 15, 2026 | 11:00 – 12:30**


In this session, you will learn how to get started with HydroServer through a practical exercise. You will work through the main steps required to add historical monitoring data to HydroServer:

- Create a **workspace**
- Add a **monitoring site**
- Create a **datastream**
- Upload **historical observations**

For this exercise, you will use the sample data that you shared with us before the workshop. The presentation uses **Rwanda** as an example, where we will upload historical stage data from the **Kanzenze station** covering the period from **1971 to 2015**. The exercises for the other countries follow the same general structure.

You can find your country's sample data in the `Exercise1/data/` folder.

### What you will create

During the exercise, you will create:

- A **workspace** where you can manage your data.
- A **monitoring site** representing the physical location where measurements are collected.
- A **datastream** containing metadata about the instrument and the measurements collected at the monitoring site.
- **Observations** corresponding to the historical measurements contained in the Excel or CSV files you provided.

For each step, we will demonstrate how the same task can be performed using:

- The **HydroServer Data Management App** in the HydroServer Playground.
- The **hydroserverpy Python package**, which allows you to interact with HydroServer programmatically.

### Follow the presentation

We will go through this [Presentation](https://www.canva.com/design/DAHRQLP5gXM/pqTYE9o6zTy-eI5wYU9MmA/edit) together step by step.

### Access Exercise 1

The Python exercise is provided as a **Jupyter Notebook** and uses the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package.

You can access and run **Exercise 1** here using binder:

👉 [**Access Exercise 1**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

You can access the exercise here if you prefer to run it in Google Colab:

👉 [**Access Exercise 1 in Google Colab**](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026?)


# Session 6a - Working with HydroServer: Automated Data Ingestion, Visualization, and Quality Control

**Tuesday, September 15, 2026 | 13:45 – 15:15**

In this session, you will learn how to continue working with data in HydroServer through a practical exercise. You will work through the main steps for automating data ingestion, visualizing your data, and performing quality control:

- Upload observations using the **Streaming Data Loader**
- Automate the upload of new observations to HydroServer
- **Visualize observations** and explore summary statistics
- Perform **Quality Control (QC)** on your observations

For this exercise, you will use the sample data that you shared with us before the workshop. The presentation uses **Rwanda** as an example. The exercises for the other countries follow the same general structure.

You can find your country's sample data in the `Exercise2/data/` folder.

### What you will do

During the exercise, you will:

- Create a **monitoring site** and a new **datastream** to receive observations.
- Configure the **Streaming Data Loader** to upload observations from a CSV file to upload new observations when the CSV file is updated.
- **Visualize your observations** in HydroServer and explore summary statistics such as the mean, median, and standard deviation.
- Use the **HydroServer Quality Control (QC) App** to review and edit your observations.

For **Rwanda**, you do not need to create a new monitoring site because the data used in Exercise 2 comes from the same physical monitoring location in Kanzenze.

For **Kenya, Uganda, and Ethiopia**, you will create a new monitoring site because the sample datasets used in Exercise 2 correspond to different monitoring locations from those used in Exercise 1.

During the Quality Control part of the exercise, you will learn how to select and filter observations using criteria such as thresholds, date ranges, and rate of change. You will also explore different operations that can be applied to selected observations, including deleting values, shifting datetimes, interpolating values, adding observations to fill gaps, and assigning data quality qualifiers.

### Follow the presentation

We will go through this [Presentation](https://www.canva.com/design/DAHRXH_5IfU/O0Qc1su_wU79mp6dOVJOxw/edit) together step by step.

### Access Exercise 2

The Python exercise is provided as a **Jupyter Notebook** and uses the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package.

You can access and run **Exercise 2** here:

👉 [**Access Exercise 2**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

# Session 7a - Querying Data and Automated Data Workflows in HydroServer  

**Wednesday, September 16, 2026 | 15:35 – 17:30**

In this session, you will learn how to retrieve the data you have uploaded to HydroServer and explore additional ways to automate data ingestion workflows. You will work through two practical exercises:

- **Query data** stored in HydroServer using Python
- Retrieve information about your **workspace, monitoring sites, datastreams, and observations**
- Explore additional approaches for **automating data ingestion workflows**

### What you will do

### Exercise 3: Querying Data from HydroServer
During the third exercise, you will use the data that you uploaded to HydroServer in the previous sessions. Using simple Python code and the **hydroserverpy** package, you will learn how to retrieve information from HydroServer and access your observations programmatically.

In this exercise, you will use the **hydroserverpy** Python package to query the data you uploaded to HydroServer during the previous exercises.

You will see examples of how to retrieve:

- Your **workspace**
- Your **monitoring sites**
- Your **datastreams**
- Your **observations**

This will show you how to access data stored in HydroServer programmatically and use it in your own Python scripts and data workflows.

### Follow the presentation

We will go through this [Presentation](https://www.canva.com/design/DAHTaSbpvA8/6u_c2D13NrFw4MAb8ujgeg/edit) together step by step.

### Access the exercises
👉 [**Access Exercise 3**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

### Exercise 4: Automating Data Ingestion Workflows

During the fourth exercise, we will explore additional approaches for **automating data ingestion workflows** and keeping observations in HydroServer up to date.

Building on the Streaming Data Loader introduced in Session 6a, we will look at additional approaches for connecting data sources to HydroServer and automatically keeping your observations up to date.

### Access the exercises
👉 [**Access Exercise 4**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)






