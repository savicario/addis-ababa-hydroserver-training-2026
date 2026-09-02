# HydroServer Training

**Workshop: Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems**

This repository contains the materials for the [HydroServer2](https://hydroserver.org/) [version v1.11.3](https://github.com/hydroserver2) training to be held in Addis Ababa, Ethiopia, on September 14–17, 2026, as part of the Workshop *"Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems"* for the National Hydrological Services of Uganda, Rwanda, Ethiopia, and Kenya. 

The HydroServer training will take place on September 15, 2026, from 8:00 AM to 5:30 PM. It will consist of four sessions of approximately 1 hour and 30 minutes each, with 20-minute breaks between sessions and a lunch break from 12:30 PM to 1:45 PM.

The training will consist of a presentation for each session, followed by hands-on exercises that we will work through together during the training. The exercises are written in Python and primarily use the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) package.

In this repository, each country has its own folder containing subfolders for Exercises 1 through 5. Each exercise folder includes the Python code and, when applicable, the sample data needed to complete the exercise.
The training will consist in a presentation for each session and exercises written in python that we will follow together during the training. In this repository, each country folder contains subfolders for the exercises from 1 to 5. Each exercise folder includes the code and in some cases sample data needed to complete the exercise.


# Session 4a - Introduction to HydroServer: Architecture, Data Models & Deployment Options 

**Tuesday, September 15, 2026 | 09:00 – 10:40**

We will go through this [Presentation](https://www.canva.com/design/DAHTaIylsx4/UT70W8BzloZcVcoe-jTBig/edit) together. The presentation will provide an introduction to HydroServer, including what HydroServer is, its main components, the types of data and formats that can be managed through HydroServer, a brief overview of possible data ingestion options, and finally, the available deployment options. We will cover these topics in this order.


# Session 5a - Getting Started with HydroServer: Setup, Data Management, and Observations

**Tuesday, September 15, 2026 | 11:00 – 12:30**


In this session, you will learn how to get started with HydroServer through a practical exercise (Exercise 1). You will work through the main steps required to set up your workspace and upload historical stage data to HydroServer:

- Create a **workspace**
- Add a **monitoring site**
- Create a **datastream**
- Upload **historical observations**

For this exercise, you will use the sample data that you shared with us before the workshop. The presentation uses **Rwanda** as an example, where we will upload historical stage data from the **Kanzenze station** covering the period from **1971 to 2015**. The stage data for this station were obtained from the [Rwanda Water Resources Portal](https://waterportal.rwb.rw/index.php/location_ng_info/259501). The exercises for the other countries follow the same structure; the only difference is that they use sample data specific to each country. You can find your country's sample data in the `Exercise1/data/` folder.

**When running the exercise code, please run each cell only once and avoid running the same cell multiple times**.

### What you will create

During the exercise, you will create:

- A **workspace** where you can manage your data.
- A **monitoring site** representing the physical location where measurements are collected.
- A **datastream** containing metadata about the instrument and the measurements collected at the monitoring site.
- **Observations** corresponding to the historical measurements contained in the CSV file you provided.

For each step, we will demonstrate how the same task can be performed using:

- The **HydroServer Data Management App** in the [HydroServer Playground](https://playground.hydroserver.org/browse).
- The **hydroserverpy Python package**, which allows you to interact with HydroServer programmatically. The package is called [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/).

### Follow the presentation

We will go through this [Presentation](https://www.canva.com/design/DAHRQLP5gXM/pqTYE9o6zTy-eI5wYU9MmA/edit) together step by step.

### Access Exercise 1

The Python exercise is provided as a **Jupyter Notebook** and uses the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package.

You can access and run **Exercise 1** here using Google Colab:

👉 <img src="https://flagcdn.com/w40/ke.png" width="28"> [Kenya: Access Exercise 1](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/kenya/Exercise1/HydroServer_Exercise1_Kenya.ipynb)

👉 <img src="https://flagcdn.com/w40/rw.png" width="28"> [Rwanda: Access Exercise 1](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/rwanda/Exercise1/HydroServer_Exercise1_Rwanda.ipynb)

👉 <img src="https://flagcdn.com/w40/ug.png" width="28"> [Uganda: Access Exercise 1](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/uganda/Exercise1/HydroServer_Exercise1_Uganda.ipynb)

👉 <img src="https://flagcdn.com/w40/et.png" width="28"> [Ethiopia: Access Exercise 1](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/ethiopia/Exercise1/HydroServer_Exercise1_Rwanda.ipynb)

If you do not have a google account, you can access the exercises through Binder:

👉 [**Access Exercise 1**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

> **Note for Ethiopia:** As I did not have access to Ethiopian data prior to the workshop, the Ethiopia exercise uses the same sample dataset and workflow as the Rwanda exercise.


# Session 6a - Working with HydroServer: Automated Data Ingestion, Visualization, and Quality Control

**Tuesday, September 15, 2026 | 13:45 – 15:15**

In this session, you will learn how to continue working with data in HydroServer through a practical exercise. You will work through the main steps for automating data ingestion from CSV files, visualizing your data, and performing quality control.

- Upload observations using the **Streaming Data Loader**
- Automate the upload of new observations to HydroServer
- **Visualize observations** and explore summary statistics
- Perform **Quality Control (QC)** on your observations

This exercise is the same for all the countries. We will use the current telemetry data from the **Kanzenze station** in Rwanda

### What you will do

During this session, you will:

- Create a **monitoring site** and a new **datastream** to receive observations.
- Configure the **Streaming Data Loader** to automatically upload new observations to HydroServer whenever the CSV file is updated.
- **Visualize your observations** in HydroServer and explore summary statistics such as the mean, median, and standard deviation.
- Use the **HydroServer Quality Control (QC) App** to review and edit your observations.

### Follow the presentation

We will go through this [Presentation](https://www.canva.com/design/DAHR4xPcFfA/avxHbnSRp74WqGka2J0IlQ/edit) together step by step.

### Access Exercise 2

This exercise will guide you through creating the monitoring site and datastream needed to load observations using the Streaming Data Loader. You will see that the process is very similar to the workflow you followed in Exercise 1. The Python exercise is provided as a **Jupyter Notebook** and uses the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package.

You can access and run **Exercise 2** here using Google Colab:

👉 <img src="https://flagcdn.com/w40/ke.png" width="28"> [Kenya: Access Exercise 2](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/kenya/Exercise2/HydroServer_Exercise2_Kenya.ipynb)

👉 <img src="https://flagcdn.com/w40/rw.png" width="28"> [Rwanda: Access Exercise 2](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/rwanda/Exercise2/HydroServer_Exercise2_Rwanda.ipynb)

👉 <img src="https://flagcdn.com/w40/ug.png" width="28"> [Uganda: Access Exercise 2](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/uganda/Exercise2/HydroServer_Exercise2_Uganda.ipynb)

👉 <img src="https://flagcdn.com/w40/et.png" width="28"> [Ethiopia: Access Exercise 2](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026/blob/main/ethiopia/Exercise2/HydroServer_Exercise2_Rwanda.ipynb)

> **Note:** For **Rwanda**, you do not need to create a new monitoring site because the data used in Exercise 2 come from the same physical monitoring location, the **Kanzenze Hydrological Station**, used in Exercise 1.
>
> For **Kenya, Uganda, and Ethiopia**, you will need to create a new monitoring site because the sample datasets used in Exercise 2 correspond to different monitoring locations from those used in Exercise 1.

You can access and run **Exercise 2** here using Binder:

👉 [**Access Exercise 2**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

Then, we will use the data uploaded to HydroServer to perform quality control and correct the observations. The Quality Control portion of the exercise will use a [demo version of the Quality Control tool](https://playground.hydroserver.org/quality-control-demo/) available in the HydroServer Playground.

During this part of the exercise, you will learn how to select and filter observations using criteria such as thresholds, date ranges, and rates of change. You will also explore different operations for reviewing and correcting selected observations, including deleting values, shifting timestamps, interpolating values, adding observations to fill data gaps, and assigning data quality qualifiers.

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

You can access and run **Exercise 3** here using Binder:

👉 [**Access Exercise 3**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

You can access the exercise here if you prefer to run it in Google Colab:

👉 [**Access Exercise 3 in Google Colab**](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026?)


### Exercise 4: Automating Data Ingestion Workflows

During the fourth exercise, we will explore additional approaches for **automating data ingestion workflows** and keeping observations in HydroServer up to date.

Building on the Streaming Data Loader introduced in Session 6a, we will look at additional approaches for connecting data sources to HydroServer and automatically keeping your observations up to date.

### Access the exercises

You can access and run **Exercise 4** here using Binder:

👉 [**Access Exercise 4**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

You can access the exercise here if you prefer to run it in Google Colab:

👉 [**Access Exercise 4 in Google Colab**](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026?)


### Exercise 5: Automating Data Uploads with HydroServer ETL Tasks

In this final exercise, we will explore how to use HydroServer ETL Tasks to automate data ingestion by creating a Data Connection.

Unlike the custom Python ETL workflow used in Exercise 4, HydroServer ETL Tasks include their own job orchestration and scheduling. Therefore, you do not need to use an external scheduler such as Windows Task Scheduler or GitHub Actions.

However, automated ETL Tasks require a deployed HydroServer instance with the orchestration system enabled. For this training, we are using the public HydroServer Playground, which does not currently have the orchestration system enabled.

Therefore, we will walk through the configuration of this exercise together, but we will not run the automated ETL Task during the training.

You can use this example after the training to configure automated data ingestion workflows on your own deployed HydroServer instance.

### Access the exercises

You can access and run **Exercise 5** here using Binder:

👉 [**Access Exercise 5**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

You can access the exercise here if you prefer to run it in Google Colab:

👉 [**Access Exercise 5 in Google Colab**](https://colab.research.google.com/github/savicario/addis-ababa-hydroserver-training-2026?)

