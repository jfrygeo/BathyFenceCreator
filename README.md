#ArcGIS Model Builder - Bathy Fence Creator

#Introduction
In order to create maritime intelligence information products, one may need to run suitbaility analyses of likely events occurring. In order to define suitable areas, one may need to pass data into a tool which gives a logistic output: 1- yes an event can occur, or 0, an event cannot occur. An example would be finding areas in bathymetry that are too shallow for a platform. A user passes a variable for the draft of the vessel into a less than or equal geoprocessing tool, and the tool finds areas that are too shallow for the vessel to operate. The output areas then could be used for further GIS analyses or converted to polygons to be used as geofences in applications such as the GeoEvent Extension for ArcGIS Server.

#Features
The Bathy Fence Creator Template includes sample data so you can easily try out the tools. 
The BathyFenceCreator folder contains sample data, a instruction document, a maps folder and a toolbox folder.

<i> Tool finds areas shallower than input depth
![](https://esri.box.com/shared/static/3ugootvigrca6p2fca9wh566oq32mdw5.png)

<i> Areas shallower than input depth <br>
![](https://esri.box.com/shared/static/1pt1ztokjl53gfyp7tyuxjycks0rdybr.png)

#Contents
|File Name | File | Description|
|-------------|------|-------------------|
|AOI.lyr |	ArcGIS layer file |	Stores the symbology and points to the dataset “AOI” in the “BathyFenceCreator.gdb” . This is used to drive the symbology of an interactive AOI operation when one uses the two tools in the toolbox.|
|Shallow Areas.lyr|	ArcGIS layer file|	Stores the symbology and points to the dataset “ShallowBathymetry” in the “BathyFenceCreator.gdb” . This is used to drive the symbology of an of the feature class outpur when one uses the two tools in the toolbox.|
|BathyExampleCA1.tif | Tif |Sample dataset obtained from NOAA National Geophysical Data Center. o	Citation: Grothe, P.G., L.A. Taylor, B.W. Eakins, K.S. Carignan, D.Z. Friday, and M. Love, 2012. Digital Elevation Models of Monterey, California: Procedures, Data Sources and Analysis, NOAA National Geophysical Data Center technical report, Boulder, CO, 15 pp.|
|BathyFenceCreator.gdb/AOI | Feature Class | An AOI feature class used to drive an “AOI” operation in the two tools in the toolbox.|
|Scratch.gdb/ShallowBathymetry | Feature Class | Output feature class showing areas that are too shallow. This is the output of both of the tools in the toolbox.|
| CreateBathyFence.mxd | Esri Map Document | Esri map document that contains the sample dataset and basemap.|
|Bathymetry Geofence Creator (Image Service Input)| ArcGIS model | Model that finds shallow areas and outputs a feature class of too shallow areas. The input in this model requires an image service. An image service example could be Esri’s TopoBathy image service.  It can be used by Esri ArcGIS Online subscribers. (http://www.arcgis.com/home/item.html?id=c753e5bfadb54d46b69c3e68922483bc)One can also publish their own image service, or WCS. This tool could be adapted to use WCS by using the “Make WCS Layer tool.”|
|Bathymetry Geofence Creator (Local Bathymetry Raster)| ArcGIS Model | Model that finds shallow areas and outputs a feature class of too shallow areas. The input is a local bathymetry raster.|

#License
Copyright 2014 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

A copy of the license is available in the repository's license.txt file.
