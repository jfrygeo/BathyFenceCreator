# Bathy Fence Creator

In order to create maritime intelligence information products, one may need to run suitbaility analyses of likely events occurring. In order to define suitable areas, one may need to pass data into a tool which gives a logistic output: 1- yes an event can occur, or 0, an event cannot occur. An example would be finding areas in bathymetry that are too shallow for a platform. A user passes a variable for the draft of the vessel into a less than or equal geoprocessing tool, and the tool finds areas that are too shallow for the vessel to operate. The output areas then could be used for further GIS analyses or converted to polygons to be used as geofences in applications such as the GeoEvent Extension for ArcGIS Server.

<i> Tool finds areas shallower than input depth
![](https://esri.box.com/shared/static/3ugootvigrca6p2fca9wh566oq32mdw5.png)

<i> Areas shallower than input depth
![](https://esri.box.com/shared/static/1pt1ztokjl53gfyp7tyuxjycks0rdybr.png)

#License
Copyright 2014 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

A copy of the license is available in the repository's license.txt file.
