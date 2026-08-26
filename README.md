# HydroServer Training

**Workshop: Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems**

This repository contains the materials for the [HydroServer](https://hydroserver.org/) version 1.11 training to be held in Addis Ababa, Ethiopia, on September 14–17, 2026, as part of the Workshop *"Piloting Interoperable Hydrometeorological Data Systems for Multi-Hazard Early Warning Systems"* for the National Hydrological Services of Uganda, Rwanda, Ethiopia, and Kenya. TThe HydroServer training will take place on September 15, 2026, and will consist of four sessions.

Each country folder in this repository contains subfolders for the exercises. Each exercise folder includes the code and sample data needed to complete the exercise.

**Session 4a - Introduction to HydroServer: Architecture, Data Models & Deployment Options ** 

**Tuesday, September 15, 2026
09:00 – 10:40**

We will go through this [Presentation](https://www.canva.com/design/DAHTaIylsx4/UT70W8BzloZcVcoe-jTBig/edit) together. The presentation will provide an introduction to HydroServer, including what HydroServer is, its main components, the types of data and formats that can be managed through HydroServer, a brief overview of possible data ingestion options, and finally, the available deployment options. We will cover these topics in this order.


**Session 5a - Getting Started with HydroServer: Setup, Data Management, and Observations** 

**Tuesday, September 15, 2026
11:00 – 12:30**

In this session, you will learn how to get started with HydroServer through a practical exercise. We will cover the key concepts that define HydroServer by creating a workspace, adding a monitoring site, creating a datastream to receive observations, and adding observations.

We will demonstrate how to complete these tasks using the HydroServer Python package, which allows you to interact with HydroServer programmatically, as well as through the HydroServer Data Management App in the HydroServer Playground.

We will go through this [Presentation](https://www.canva.com/design/DAHRQLP5gXM/pqTYE9o6zTy-eI5wYU9MmA/edit) together step by step.
 
 The presentation uses Rwanda as an example, where we upload stage data from the Kanzenze station covering the period from 1971 to 2015. The exercises for the other countries follow a similar structure.

  In this exercise, you will create your own *workspace* to manage your data, a *monitoring site* representing the physical location where measurements are collected, a *datastream* containing metadata about the instrument taking measurements at the monitoring site, and *observations* corresponding to the measurements in the Excel and CSV files you shared with us before the workshop. If you navigate to the `Exercise1/data/` folder, you will find the sample data you shared with us.

  The code is written in Python in Jupyter Notebooks with the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package. You can access and run Exercise 1 here: [Access Exercise 1](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)

- **Exercise 2: Other Methods to Load Observations into HydroServer:** See the [Presentation](https://www.canva.com/design/DAHRXH_5IfU/O0Qc1su_wU79mp6dOVJOxw/edit) for instructions. We will go through the presentation and complete the exercise together during the second session of the workshop.

  In this exercise, you will upload observations using the [**Streaming Data Loader**](LINK). The Streaming Data Loader is a HydroServer tool that monitors a CSV file for new sensor observations and automatically uploads new data to a HydroServer datastream as the file is updated.

  To load data using the Streaming Data Loader, you need to repeat some of the steps completed in Exercise 1, particularly creating a monitoring site and a new datastream to receive the data. In the case of Rwanda, we do not need to create a new monitoring site because the new station is located at the same physical site in Kanzenze.

  For Kenya, Uganda, and Ethiopia, you will need to create a new monitoring site because, in Exercise 1, you used your own sample datasets from different monitoring locations.

  You can access the exercise by going to your country folder and opening Exercise 2. The code is written in Python in Jupyter Notebooks with the [hydroserverpy](https://hydroserver.org/user-guides/tutorials/getting-started-with-hydroserverpy/) Python package. You can access the GitHub repository and run the exercise here: [Access Exercise 2](https://mybinder.org/v2/gh/savicario/addis-ababa-hydroserver-training-2026/main?urlpath=lab)


**Session 6a - Data visualization, Quality Analysis, and Accessing** 

**Tuesday, September 15, 2026
13:45 – 15:15**

- **Exercise 3: Data Quality Analysis in HydroServer:** See the [Presentation](https://www.canva.com/design/DAHR4xPcFfA/avxHbnSRp74WqGka2J0IlQ/edit) for instructions.



