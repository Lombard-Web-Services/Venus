# Venus maps with elevation
Here is 2 interactive maps of the surface of Venus, the data retrieved is coming from the NASA public website. The elevation data was extracted from the imagery that the Magellan JPL USGS team has distributed during the Parker's Solar probe flyby on 2021-02-20 at 20:11:30 UTC. The topographical radar view I called "geoid" into the script was shot partly in the 1990s, the other half of the view has been updated by the WISPR instrument of the Parker's Solar Probe in 2021.

## Venus Geoid Topography
![image](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/demo/Venus_geoide.gif)

I used [GDAL](https://gdal.org/) as well as [itowns-project](https://www.itowns-project.org/ "itowns project") for the post-processing of the files and in order to allow a 3-dimensional visualization of the surface of Venus. I have treated the source of the elevation file as a geoid file and translated it to geotiff 1 channel to apply the Z-factor feature.

## Venus surface elevation
![image](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/demo/Venus_surface.gif)

The second part of this work was to add a 2nd layer (FLOAT32) to the first elevation surface, by doing this we can see a textured version of the planet's ground.

## Demo
html files :
* [venus-geoide.min.html](https://lombard-web-services.github.io/Venus/Venus/venus-geoide.min.html) Interactive map minified version of the planet Venus with rgb geoid (1232px x 616px).
* [venus-geoide](https://lombard-web-services.github.io/Venus/Venus/venus-geoide.html) Interactive map version of the planet Venus with rgb geoid (1232px x 616px).
* [venus-terrain.min.html](https://lombard-web-services.github.io/Venus/Venus/venus-terrain.min.html) Interactive map minified version of the planet Venus with surface texture(4096px x 2048px).
* [venus-terrain.html](https://lombard-web-services.github.io/Venus/Venus/venus-terrain.html) Interactive map version of the planet Venus with surface texture(4096px x 2048px).


## Images source files
The most useful images sources are into the sources folder
[Venus.tif](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/sources/Venus.tif) TIF file of the Venus Topography.
[Venus-terrain](https://github.com/Lombard-Web-Services/Venus/raw/master/Venus/sources/Venus-terrain.png) PNG file of the Venus surface.


## Credits & License
Dataset : Parker Solar Probe, Magellan Team/JPL/USGS 
Post processing tools : IGN, model (CNES/GRGS and GFZ), gdal, itowns

Credits scripts used: 
* [itowns-project](https://www.itowns-project.org/ "itowns project") MIT, Cecill V2 license
* [gdal](https://gdal.org/) MIT license
* dat.gui.js Copyright 2011 Data Arts Team, Google Creative Lab Licensed under the Apache License, Version 2.0 (the "License")

### MIT License

Copyright (c) 2023 Thibaut Lombard (contact@lombard-web-services.com)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
