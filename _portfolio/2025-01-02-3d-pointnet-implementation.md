---
title: "3D PointNet++ Implementation for Smart Construction Management"
excerpt: "A CPU-only PointNet++ (SSG) pipeline for semantic segmentation of building elements from 3D point clouds, supporting real-time construction progress monitoring.<br/><img src='/images/portfolio/pointnet.jpg'>"
collection: portfolio
permalink: /portfolio/2025-01-02-3d-pointnet-implementation
date: 2025-01-02
---

**Duration:** 3 years · **Repo:** [github.com/LitonSarker/3dPointNetImplementation](https://github.com/LitonSarker/3dPointNetImplementation)

### Introduction

Construction projects often lack reliable and updated BIM models, which makes manual progress tracking costly and inefficient. 3D point clouds provide an alternative by capturing as-built conditions. This project demonstrates an automation pipeline using PointNet++ to segment building elements from point cloud data, supporting real-time progress monitoring.

**Target audience:** researchers, industry engineers, and PhD advisors interested in computer vision and construction management.

### ✨ Features

* CPU-only implementation of PointNet++ (SSG) for semantic segmentation
* Supports XYZ or XYZ+RGB features
* Automatic train/validation split (80:20) from raw S3DIS dataset
* Tracks progress via OA, mAcc, mIoU metrics
* Checkpointing (`last_model.pth`, `best_model.pth`) and logging (`history.json`, `train_log.json`)
* Preprocessing scripts to convert S3DIS annotations → PLY files

### 🏗️ Applications in Construction

* Real-time progress monitoring from 3D point clouds
* Comparison of as-built vs BIM models (or pseudo-BIM)
* Detecting installed vs missing elements on site
* Compatible with data from LiDAR, CCTV, drones
