# old-maps
Georeferencing old, scanned maps of San Mateo County

## Introduction
The [San Mateo County Department of Planning and Building](http://planning.smcgov.org/) has scaned about 125 old maps from its paper map collection. Rather than letting these digital maps gather dust on hard drives, we're georeferencing these maps and making as many of them available to the public as possible.

## The Work
Georeferencing is the process of assigning spatial coordinates to data that is spatial in nature, but has no explicit geographic coordinate system. Here, we will take scanned map images from the County and add them to a base map in QGIS.

## Steps
1. [Download QGIS](http://www.qgis.org/en/site/forusers/download.html) if you need it
1. Review the georeferencing steps on the [QGIS Georeferencer documentation](https://docs.qgis.org/2.2/en/docs/user_manual/plugins/plugins_georeferencer.html)
1. Find a map you'd like to georeference on the [OpenSMC Google Drive](https://drive.google.com/open?id=0B4abucxuAKOWSlVvaE5JWjFkdE0)
1. Download the image file from Google Drive
1. Download the [QGIS project file](https://github.com/opensmc/old-maps/blob/master/old_maps_qgis_project.zip) that contains the base layers you'll use to geocode to from [Google Drive](need link)
1. Open the project in QGIS to get started georeferencing
1. When you finish, make sure to upload the [Finished folder](https://drive.google.com/drive/folders/0B4abucxuAKOWc0ktZWg4TkNRWHM?usp=sharing) on the OpenSMC Google Drive

## Advice
* If you create at least 6 control points as evenly distributed across the image as possible, the georeferenced map won't look warped
* Use second order polynomial as a transformation setting
* Feel free to skip maps you don't like, someone else will work on it
* Some maps can't be georefenced because they are a small portion of the sheet. Please feel free to skip these, but let John know (comments in Github repo is great)
* For more information on georeferencing in QGIS, take a look at [this video] (https://www.youtube.com/watch?v=KBBepLyyGL8)
* If you have any questions or comments at all, please don't hesitate to ask! [@jridener](https://opensmc.slack.com/) on Slack and jridener@opensmc.org
