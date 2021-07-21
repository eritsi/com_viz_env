# Community Visualization development environment

![image](https://user-images.githubusercontent.com/40695945/126501219-48e49907-5ca7-4456-8fa4-6f789526e0c1.png)

This repository provides a development environment on GitPod for developping plots and charts in Google Data Portal (Data Studio).
As of July 2021, the official distribution contains some errors  and need to fix [the issue #190](https://github.com/googledatastudio/tooling/issues/190)

For those who want to concentrate the own charts for Data Portal, this repository allows to provide all-in-one environment in a browser tab such as Google Chrome.

## Prerequisite

* GitHub account
* GitPod account ([https://gitpod.io/login](https://gitpod.io/login))

## Quick Start
Open the following link in your tab browser.
[https://gitpod.io/#https://github.com/eritsi/com_viz_env](https://gitpod.io/#https://github.com/eritsi/com_viz_env)

### ToDo in initialization workflows
```
# 1st workflow on the left split terminal
# This workflow installs D3.js, Chart.js and gsutil
1. Open the gsutil configuration link with Command+Click (as guided in your terminal)
2. Select your account and authorize gsutil functions
3. Copy & Paste your token
4. Specify your GCP Project ID (Your Plot source codes for Data Portal will be stored)
5. y/N question for Google statistics
```
```
# 2nd workflow on the middle split terminal
# This workflow installs npx @google/dscc-gen viz
1. Y/n question for Google statistics
2. Name a working directory
2. Give a GCS bucket path for development
3. Give a GCS bucket path for production
```
```
# 3rd workflow on the right split terminal
# This workflow fix the issue #190 and npm run start 
```
```
# Simple Browser in the Browser tab
Even if the Port 8080 looks closed, try to refresh the simple Browser at the end of workflows. Normally local development browser will be shown.
```

## How to develop new plots for DataPortal

[The official codelab](https://codelabs.developers.google.com/codelabs/community-visualization-dscc-gen#0) provides training.
