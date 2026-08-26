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

### Follow the presentation

We will go through this [Presentation](https://www.canva.com/design/DAHRQLP5gXM/pqTYE9o6zTy-eI5wYU9MmA/edit) together step by step.

For each step, we will demonstrate how the same task can be performed using:

- The **HydroServer Data Management App** in the HydroServer Playground.
- The **hydroserverpy Python package**, which allows you to interact with HydroServer programmatically.

### Access Exercise 1

The Python exercise is provided as a **Jupyter Notebook** and uses the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package.

You can access and run **Exercise 1** here:

👉 [**Access Exercise 1**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)


# Session 6a - Working with HydroServer: Automated Data Ingestion, Visualization, and Quality Control

**Tuesday, September 15, 2026 | 13:45 – 15:15**

In this session, you will learn how to work with data in HydroServer after completing the initial setup in Exercise 1. We will focus on three main tasks:

- Automating data ingestion using the **Streaming Data Loader**
- Exploring and **visualizing observations** in HydroServer
- Performing **Quality Control (QC)** on your observations

We will go through this [Presentation](https://www.canva.com/design/DAHRXH_5IfU/O0Qc1su_wU79mp6dOVJOxw/edit) together step by step.

### Exercise 2: Automated Data Ingestion with the Streaming Data Loader

In this exercise, you will upload observations using the **Streaming Data Loader**. The Streaming Data Loader is a HydroServer tool that can be used to automatically upload observations from CSV files stored and updated on your computer.

We will show you how to configure the Streaming Data Loader so that new observations can be uploaded to HydroServer as the CSV file is updated.

To use the Streaming Data Loader, you will repeat some of the steps from Exercise 1, particularly creating a **monitoring site** and a new **datastream** to receive the observations.

For **Rwanda**, you do not need to create a new monitoring site because the data used in Exercise 2 comes from the same physical monitoring location in Kanzenze.

For **Kenya, Uganda, and Ethiopia**, you will create a new monitoring site because the sample datasets used in Exercise 2 correspond to different monitoring locations from those used in Exercise 1.

You can find Exercise 2 in your country's folder. The exercise is provided as a **Jupyter Notebook** and uses the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package.

You can access and run **Exercise 2** here:

👉 [**Access Exercise 2**](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

### Data Visualization

Once the observations have been uploaded, we will explore how to **visualize the data in HydroServer**. We will also review some of the summary statistics provided by HydroServer, including the **mean, median, and standard deviation**.

### Quality Control

Finally, we will work together with the **HydroServer Quality Control (QC) App** to explore different ways of reviewing and editing observations.

You will learn how to filter and select observations using criteria such as:

- Thresholds
- Date ranges
- Rate of change

You will then learn how to perform different QC operations on the selected observations, including:

- Deleting values
- Shifting observation datetimes
- Interpolating values
- Adding observations to fill data gaps
- Assigning data quality qualifiers to observations


