# STAPull
STAPull analysis code 

STAPull analysis for processing ONI files. 

1. ONI pre-processing
An ImageJ macro that parses ome-xml metadata description and adds tags to tiff header for future referencing via 'image info' panel in ImageJ.
Separates channels, calibrates scale and saves as .tiff in specified location.

2. Channel registration
A python script that uses the img_dft library (https://pypi.org/project/imreg_dft/) to align left and right ONI images based on ground-truth Tetraspeck data

3. Coincidence detection
An ImageJ macro that uses the ComDet plugin for Fiji (https://github.com/ekatrukha/ComDet) to batch detect and report single channel and coincident puncta.

4. Process CSVs
A python script to compile and organise outputs from the coincidence detection
