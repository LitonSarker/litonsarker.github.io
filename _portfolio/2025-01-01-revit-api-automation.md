---
title: "Revit API Automation — AI for Smart Construction Progress Monitoring"
excerpt: "Automates isolation, visualization, and quantification of Revit model elements with screenshot/CSV export and 3D point cloud dataset generation for construction progress tracking.<br/><img src='/images/portfolio/revit-api-automation.jpg'>"
collection: portfolio
permalink: /portfolio/2025-01-01-revit-api-automation
date: 2025-01-01
---

**Duration:** 3 years · **Repo:** [github.com/LitonSarker/RevitAPIAutomation](https://github.com/LitonSarker/RevitAPIAutomation)

### Introduction

This tool helps automate isolation, visualization, and quantification of Revit model elements with automatic screenshot and CSV export and 3D point cloud dataset generation that works as a data pipeline for Construction Progress Tracking.

Built using pyRevit API and IronPython, this tool forms the Ground Truth (GT) dataset for comparing as-built 3D point clouds generated from site data (e.g., LiDAR, photogrammetry). It is part of a larger ongoing research framework toward automated construction progress monitoring and pseudo-BIM generation under the LSU Construction Management research collaboration.

**Tools & technologies:** Revit, RevitAPI, pyRevit, IronPython

### ✨ Main Features

* Isolate Architectural / Structural / MEP categories
* Automatic screenshot capture for isolated model views
* Export CSV summary of element categories and counts
* Auto-copy element IDs to clipboard after each isolate operation
* Extract 3D coordinates (in project units) of each element
* Support for linked Revit models

{% include figure image_path="/images/Revit_Automation_UI.png.png" alt="Project Screenshot" caption="Fig: Revit Automation Tool UI" %}
