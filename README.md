# old-maps

Georeferencing old, scanned maps of San Mateo County

## Introduction

The [San Mateo County Department of Planning and
Building](http://planning.smcgov.org/) has scaned about 125 old maps
from its paper map collection. Rather than letting these digital maps
gather dust on hard drives, we're georeferencing these maps and making
as many of them available to the public as possible.

## The Work

Georeferencing is the process of assigning spatial coordinates to data
that is spatial in nature, but has no explicit geographic coordinate
system. Here, we will take scanned map images from the County and add
them to a base map in QGIS.

## Steps

1. [Download QGIS](http://www.qgis.org/en/site/forusers/download.html)
    if you need it

1. Review the georeferencing steps on the
    [QGIS Georeferencer documentation](https://docs.qgis.org/2.2/en/docs/user_manual/plugins/plugins_georeferencer.html)

1. Find a map you'd like to georeference on the
    [OpenSMC Google Drive](https://drive.google.com/open?id=0B4abucxuAKOWSlVvaE5JWjFkdE0)

1. Edit the "who is working on what" spreadsheet on Google Drive to
    add your name, and make sure no one else is already working on
    that map.
    [old maps spreadsheet](https://docs.google.com/spreadsheets/d/1tC7ryn8hPdPzYAco3cXPgJXA8C87hgGQNNUfyiRUT-s/edit#gid=0)

1. Download the image file from Google Drive

1. Download the
    [QGIS project file](https://github.com/opensmc/old-maps/blob/master/old_maps_qgis_project.zip)
    that contains the base layers you'll use. (Your raster map will align to one or more of these base
    layers.) If you prefer to work with git, you can use git clone https://github.com/opensmc/old-maps.git
    to check out the whole project, including this README.

1. Open the project in QGIS to get started georeferencing

1. When you finish, make sure to upload the
    [Finished folder](https://drive.google.com/drive/folders/0B4abucxuAKOWc0ktZWg4TkNRWHM?usp=sharing)
    on the OpenSMC Google Drive, and remove the original map from the top folder.

1. As a final step, update the "who is working on what" spreadsheet to mark the map complete.
    [old maps spreadsheet](https://docs.google.com/spreadsheets/d/1tC7ryn8hPdPzYAco3cXPgJXA8C87hgGQNNUfyiRUT-s/edit#gid=0)


## Advice

* The county vector maps are in web mercator / pseudo mercator, EPSG:3857.

* When QGIS prompts for the raster coordinate system, EPSG:3493 (Cal Zone 3)
   is not a bad guess. [Description of EPSG:3493](https://epsg.io/3493)

* If you create at least 6 control points as evenly distributed across
   the image as possible, the georeferenced map won't look warped

* Use second order polynomial as a transformation setting

* Feel free to skip maps you don't like, someone else will work on it

* Some maps can't be georefenced because they are a small portion of
   the sheet. Please feel free to skip these, but let John know
   (comments in Github repo is great)

* If a "map" is a actually a page with a lot of non-map content and a small
   map somewhere in the page, consider clipping the original "map" file to
   just the map, and geo-refererencing the clipped image. Save the clipped
   image as the original filename with "_clipped" and store both the clipped
   and the original files on the the google drive when done.

* For more information on georeferencing in QGIS, take a look at
   [this video](https://www.youtube.com/watch?v=KBBepLyyGL8)

* If you have any questions or comments at all, please don't hesitate to ask!
    [@jridener](https://opensmc.slack.com/) on Slack and jridener@opensmc.org
