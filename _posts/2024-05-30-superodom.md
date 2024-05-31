---
layout: post
title: "Super odometry: IMU-centric LiDAR-visual-inertial estimator for challenging environments"
date: 2024-05-30 12:00:01
categories: research
description: "We propose Super Odometry, a high-precision multi-modal sensor fusion framework, providing a simple but effective way to fuse multiple sensors such as LiDAR, camera, and IMU sensors and achieve robust state estimation in perceptually-degraded environments. Different from traditional sensor-fusion methods, Super Odometry employs an IMU-centric data processing pipeline, which combines the advantages of loosely coupled methods with tightly coupled methods and recovers motion in a coarse-to-fine manner."
author: "Shibo Zhao"
published: true
redirect: "https://superodometry.com/"

show_sidebar: false
# slim_content_width: true
permalink: /superodom/
image: /img/posts/2024-05-30-superodom/superodom.png
datatable: true
title_image: None
hero_image: /img/posts/2024-05-30-superodom/superodom_hero.png
hero_height: is-large
remove_hero_title: true
menubar_toc: true

tags: Learning, Perception, SLAM
---

We propose Super Odometry, a high-precision multi-modal sensor fusion framework, providing a simple but effective way to fuse multiple sensors such as LiDAR, camera, and IMU sensors and achieve robust state estimation in perceptually-degraded environments. Different from traditional sensor-fusion methods, Super Odometry employs an IMU-centric data processing pipeline, which combines the advantages of loosely coupled methods with tightly coupled methods and recovers motion in a coarse-to-fine manner. The proposed framework is composed of three parts: IMU odometry, visual-inertial odometry, and laser-inertial odometry. The visual-inertial odometry and laser-inertial odometry provide the pose prior to constrain the IMU bias and receive the motion prediction from IMU odometry. To ensure high performance in real-time, we apply a dynamic octree that only consumes 10 % of the running time compared with a static KD-tree. The proposed system was deployed on drones and ground robots, as part of Team Explorer’s effort to the DARPA Subterranean Challenge where the team won 1st and 2nd place in the Tunnel and Urban Circuits, respectively.