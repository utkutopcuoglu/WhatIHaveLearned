---
title: "EOD 12.09.2021"
description: "My daily work report"
layout: post
toc: false
comments: true
# image: images/some_folder/your_image.png
hide: true # hide from homepage
search_exclude: true # set the front matter search_exclude to false if you don't want users to find your hidden post in a search.
categories: [Daily Work Reports] # Add tags to table of content
# You can toggle the display of tags on/off by setting show_tags to true or false in _config.yml:
# Set this to true to display tags on each post
# show_tags: true
metadata_key1: metadata_value1
metadata_key2: metadata_value2
---


## Tasks Completed:
- combine weeks 1-2 to 1-6 and run 2 detection models on it and generate gt and prediction .csv files.
- Updated yolo-wild results with grids , true alert and false positives (date is removed but not updated on all dataset results). True alert and false positives worked only on single class -> fixed for multiple.
- Minor fix in reverse ssh readme.
 
## Problems Identified:
- Yesterday I had a update issue on ubuntu (guess after I messed up with packages). Then today ubuntu could not boot until ~11:00 . I had to enter recovery mode and remove, clean purges, update etc, than the problem got fixed (do not know real cause or why it got solved).
- VSCode ipynb plugin did not work due to kernel issues (Python package was not working correct). I uninstalled and deleted the folder in .vscode , then when I re-installed it worked fine.
 
## Incomplete tasks and their state:
- combine week csv files and automate it, run yolo and detection on it
- Generate predict csv for yolov5 on week 1-2 to 1-6 combined.
- Make progress in fastai
 
