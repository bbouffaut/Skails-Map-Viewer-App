<h1 align="center">Skails Map Viewer</h1>

Skails Map Viewer is an All-In-One app that provides **full-screen easy-to-switch topo maps** from various providers, and key features to plan and drive any outdoor activities in the world (Hiking, Trail Running, Ski Touring, Alpinism,...) 

It can be installed from here [![Google Play](html/google-play-badge_small.png)](https://play.google.com/store/apps/details?id=com.skails.opentopomapviewer)

It has been developed from [osmdroid demo project](https://github.com/osmdroid/osmdroid)



# Overall Presentation

- The main screen is a simple full-screen map interface

<p align="center">
<img src="html/screenshot-mainmap-opentopomap.png" alt="drawing" width="300"/>
</p>

- Different map sources can be selected to be easily displayed in the main map

<p align="center">
<img src="html/screenshot-tilessources-list.png" alt="drawing" width="300"/>
</p>

- An auto-completed location search function permits to center the main map everywhere in the world

<p align="center">
<img src="html/screenshot-location-search.png" alt="drawing" width="300"/>
</p>

<br><br>

# Main Screen Buttons

The main screen of the app is a full-screen map with:
- Minimap that provides an overall situation of the displayed scene
- A compas
- Some buttons that permit to easily control the map and add some overlays

Here is a description of those buttons:

| Icon                                                  | Signification |
|-------------------------------------------------------|---------------|
| <img src="html/ic_settings_icon_.png"> | Access the app Main menu (including the Tiles Sources list selection)|
| <img src="html/ic_search.png"> | Search for a location to center the map on|
| <img src="html/ic_rotation.png"> | Change the Map source: 1 press switch to the next Tile Source in the configuration list |
| <img src="html/ic_position_3.png"> | Center the map on the current location (Need location persmission to be granted |
| <img src="html/ic_slopes_inclination_dynamit.png"> | Display slopes inclination overlay on top of main map (<b>FRANCE ONLY</b>). Successive presses on the button increase the contrast of the overlay |
| ![Follow-Me](html/ic_follow_me.png) | Activate Follow-Me service. Your moves are recorded and displayed on the Main Map. Works as a ForeGround service (with notification in the icons tray to control it) |
| <img src="html/ic_weather_.png"> | Display Weather information as overlays of Main Map. Successive press switch the overlay type: pressure, precipitations, temperature |


<br><br>

# Map Tiles Sources

Different Map Tiles Sources are accessible via the application. Please refer to the Tiles Source warning

| Tile Source            | Screenshot | Usage |
|------------------------|------------|-------|
|Map |<img src="html/screenshot-mainmap-opentopomap.png" alt="drawing" width="200"/> |CC-BY-SA licence |
|IGN Scan25Tour |<img src="html/screenshot-mainmap-ign-scan25tour.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|IGN Maps |<img src="html/screenshot-mainmap-ign-maps.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|IGN PLAN v2 |<img src="html/screenshot-mainmap-ign-planv2.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|OpenStreetMap (Mapnik) |<img src="html/screenshot-mainmap-mapnik.png" alt="drawing" width="200"/> |Open Data Commons Open Database License (ODbL) by the OpenStreetMap Foundation (OSMF) |
|Mapbox Outdoors  |<img src="html/screenshot-mainmap-mapbox-outdoor.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|Mapbox Streets |<img src="html/screenshot-mainmap-mapbox-streets.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|Bing Maps |<img src="html/screenshot-mainmap-bings.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|Mapbox Satellite (with streets)|<img src="html/screenshot-mainmap-mapbox-satellite-streets.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|Thunderforest Cycle |<img src="html/screenshot-mainmap-thunderforest-cycle.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |
|MapTiler Topographic |<img src="html/screenshot-mainmap-maptiler-topographique.png" alt="drawing" width="200"/> |NOT FREE (<b>May stop working at any time</b>) |

<br><br>

# Slope Inclination Overlay (FOR FRANCE ONLY)

When clicking the <img src="html/ic_slopes_inclination_dynamit.png"> button, the Slopes Inclination overlay displays on top of Main Map. When pressing the button several times, the contrast of the overlay increases

| 1 Press | 2 Presses | 3 Presses |
|---------|-----------|-----------|
|<img src="html/screenshot-mainmap-inclination-press-1.png" alt="drawing" width="200"/> | <img src="html/screenshot-mainmap-inclination-press-2.png" alt="drawing" width="200"/> | <img src="html/screenshot-mainmap-inclination-press-3.png" alt="drawing" width="200"/> |

<br><br>

# Weather Overlay

When clicking the <img src="html/ic_weather_.png" alt="drawing" width="42" height="42"/> button, some Weather information overlay displays on top of Main Map. When pressing the button several times, different weather information appears

| 1 Press: Temperatures | 2 Presses: Pressions | 3 Presses: Precipitations |
|---------|-----------|-----------|
|<img src="html/screenshot-mainmap-weather-temperature.png" alt="drawing" width="200"/> | <img src="html/screenshot-mainmap-weather-pressure.png" alt="drawing" width="200"/> | <img src="html/screenshot-mainmap-weather-precipitations.png" alt="drawing" width="200"/> |

<br><br>

# Follow Me Service

When clicking the ![Follow-Me](html/ic_follow_me.png) button, the Follow-Me Service starts. Then:
- The Button changes for  ![Follow-Me running](html/ic_follow_me_on.png) indicating that the service is running
- Notifcation appears in the icon tray
- Red lines is displayed to follow your position updates

<p align="center">
 <img src="html/screenshot-followme-run.png" alt="drawing" width="300"/>
 </p>

- To stop the Follow-Me service, press again on the ![Follow-Me running](html/ic_follow_me_on.png) button. It then switches back to  ![Follow-Me](html/ic_follow_me.png)
- To reset the Follow-Me service, long-press on the ![Follow-Me](html/ic_follow_me.png) button

<br><br>

# Itinary Service

- When long-pressing anywhere on the map, a ![Start Itinary](html/ic_set_position.png) icon appears. It marks the start of an itinary computation
- When pressing anywhere on the map, a ![Itinary Waypoint](html/marker_default.png) icon appears that mark a waypoint on the itinary computation
- When long-pression again, a ![Start Itinary](html/ic_set_position.png) icon appears. It marks the end of the itinary computation. Then Itinary Proposal including itinary information (Distance, walking duration, Elevation) displays

<p align="center">
 <img src="html/screenshot-mainmap-itinary.png" alt="drawing" width="300"/>
 </p>

# BERA display
######For France only: Bulletin d'Estimations des Risques d'Avalanche

- When pressing anywhere on the map, IF EXISTS, the BERA of the massif you touch displayed in full-screen

<p align="center">
 <img src="html/Screenshot_20221119-110938_Skails Map Viewer.jpg" alt="drawing" width="300"/>
 </p>