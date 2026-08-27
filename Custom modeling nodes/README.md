SAS Viya Forecasting Custom Modeling Nodes
==========================================

## Overview
The following files are required to define a pluggable modeling strategy in SAS Visual Forecasting 8.3:
1. code.sas, which contains the SAS® code to be executed
2. validation.xml, which defines the validation rules for the strategy specification settings (properties)
3. template.json, which defines the metadata of the strategy

Starting from SAS Visual Forecasting 8.4, another file is required, metadata.json. This file guarantees that the version of the modeling strategies matches the current version of Model Studio. You can download an existing strategy from the exchange and copy the metadata.json file to your modeling strategy to make sure you have the correct version.

These files are packed in a .zip file for uploading to or downloading from The Exchange in SAS Visual Forecasting. You can download an existing pluggable modeling strategy and learn from the downloaded example files. Then you can modify the contents accordingly and use the modified files.

This repository currently includes the [Custom Seasonal Modeling Node](Seasonal_Model/README.md), which demonstrates node-level event definitions and BY-group-aware event usage mapping.