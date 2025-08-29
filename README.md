# 🪐 Venus maps with elevation 
Here is 2 interactive maps of the surface of Venus, the data retrieved is coming from the NASA public website. The elevation data was extracted from the imagery that the Magellan JPL USGS team has distributed during the Parker's Solar probe flyby on 2021-02-20 at 20:11:30 UTC, that seems to be an enhanced version of Magellan Global C3-MDIR topography dating of 1990's. 

## 🔭 Venus Geoid Topography 
![image](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/demo/Venus_geoide.gif)

I used [GDAL](https://gdal.org/) as well as [itowns-project](https://www.itowns-project.org/ "itowns project") for the post-processing of the files and in order to allow a 3-dimensional visualization of the surface of Venus. I have treated the source of the elevation file as a geoid file and translated it to geotiff 1 channel to apply the Z-factor feature.

## ⛰️ Venus surface elevation
![image](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/demo/Venus_surface.gif)

The second part of this work was to add a 2nd layer (FLOAT32) to the first elevation surface, by doing this we can see a textured version of the planet's ground.

## 🖥️ Demo
html files :
* [venus-geoide.min.html](https://lombard-web-services.github.io/Venus/Venus/venus-geoide.min.html) Interactive map minified version of the planet Venus with rgb geoid (1232px x 616px).
* [venus-geoide](https://lombard-web-services.github.io/Venus/Venus/venus-geoide.html) Interactive map version of the planet Venus with rgb geoid (1232px x 616px).
* [venus-terrain.min.html](https://lombard-web-services.github.io/Venus/Venus/venus-terrain.min.html) Interactive map minified version of the planet Venus with surface texture(4096px x 2048px).
* [venus-terrain.html](https://lombard-web-services.github.io/Venus/Venus/venus-terrain.html) Interactive map version of the planet Venus with surface texture(4096px x 2048px).


## 📸 Images source files
The most useful images sources are into the sources folder
[Venus.tif](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/sources/Venus.tif) TIF file of the Venus Topography.
[Venus-terrain.png](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/sources/Venus-terrain.png) PNG file of the Venus surface.


## ⚖️ Credits & License
Dataset : Parker Solar Probe, Magellan Team/JPL/USGS 
Post processing tools : IGN, model (CNES/GRGS and GFZ), gdal, itowns

Credits scripts used: 
* [itowns-project](https://www.itowns-project.org/ "itowns project") MIT, Cecill V2 license
* [gdal](https://gdal.org/) MIT license
* dat.gui.js Copyright 2011 Data Arts Team, Google Creative Lab Licensed under the Apache License, Version 2.0 (the "License")

### License: CC BY-NC-ND
Author: Thibaut Lombard
Dataset: Parker Solar Probe, Magellan Team/JPL/USGS
Post processing tools: IGN, model (CNES/GRGS and GFZ), gdal, itowns

Credits scripts used: * itowns-project MIT, Cecill V2 license

gdal MIT license

dat.gui.js Copyright 2011 Data Arts Team, Google Creative Lab Licensed under the Apache License, Version 2.0 (the "License")

## 📜 License & Author 

**License:** 
![Logo de la licence CC BY-NC-ND](CC_BY-NC-ND.png)

**Author:** Thibaut LOMBARD

**GitHub:** [https://github.com/Lombard-Web-Services](https://github.com/Lombard-Web-Services)

**Project Repository:** [Venus](https://github.com/Lombard-Web-Services/Venus)

**Alias:** [@lombardweb](https://x.com/lombardweb)



## ⚖️ License Details 

This work is licensed under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License**. To view a copy of this license, visit [http://creativecommons.org/licenses/by-nc-nd/4.0/](http://creativecommons.org/licenses/by-nc-nd/4.0/) or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

The main conditions of this license are:

* **Attribution (BY):** You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
* **NonCommercial (NC):** You may not use the material for commercial purposes.
* **NoDerivatives (ND):** If you remix, transform, or build upon the material, you may not distribute the modified material.
