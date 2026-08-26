# HydroServer Training

**Workshop: Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems**

This repository contains the materials for the [HydroServer](https://hydroserver.org/) version 1.11 training to be held in Addis Ababa, Ethiopia, on September 14–17, 2026, as part of the Workshop *"Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems"* for the National Hydrological Services of Uganda, Rwanda, Ethiopia, and Kenya. TThe HydroServer training will take place on September 15, 2026, and will consist of four sessions.

Each country folder in this repository contains subfolders for the exercises. Each exercise folder includes the code and sample data needed to complete the exercise.


# Session 4a - Introduction to HydroServer: Architecture, Data Models & Deployment Options 

**Tuesday, September 15, 2026 |  09:00 – 10:40**
---

We will go through this [Presentation](https://www.canva.com/design/DAHTaIylsx4/UT70W8BzloZcVcoe-jTBig/edit) together. The presentation will provide an introduction to HydroServer, including what HydroServer is, its main components, the types of data and formats that can be managed through HydroServer, a brief overview of possible data ingestion options, and finally, the available deployment options. We will cover these topics in this order.


# Session 5a - Getting Started with HydroServer: Setup, Data Management, and Observations

**Tuesday, September 15, 2026 | 11:00 – 12:30**

---

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


## Session 6a - Working with HydroServer: Automated Data Ingestion, Visualization, and Quality Control  

**Tuesday, September 15, 2026
13:45 – 15:15**


- **Exercise 2: Other Methods to Load Observations into HydroServer:** See the [Presentation](https://www.canva.com/design/DAHRXH_5IfU/O0Qc1su_wU79mp6dOVJOxw/edit) for instructions. We will go through the presentation and complete the exercise together during the second session of the workshop.

  In this exercise, you will upload observations using the [**Streaming Data Loader**](LINK). The Streaming Data Loader is a HydroServer tool that monitors a CSV file for new sensor observations and automatically uploads new data to a HydroServer datastream as the file is updated.

  To load data using the Streaming Data Loader, you need to repeat some of the steps completed in Exercise 1, particularly creating a monitoring site and a new datastream to receive the data. In the case of Rwanda, we do not need to create a new monitoring site because the new station is located at the same physical site in Kanzenze.

  For Kenya, Uganda, and Ethiopia, you will need to create a new monitoring site because, in Exercise 1, you used your own sample datasets from different monitoring locations.

  You can access the exercise by going to your country folder and opening Exercise 2. The code is written in Python in Jupyter Notebooks with the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package. You can access the GitHub repository and run the exercise here: [Access Exercise 2](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)





