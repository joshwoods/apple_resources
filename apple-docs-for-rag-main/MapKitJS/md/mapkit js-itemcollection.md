

- MapKit JS
-  ItemCollection 

Class

# ItemCollection

A tree structure containing annotations, overlays, and nested item collection objects.

MapKit JS 5.0+

``` source
interface ItemCollection
```

## Overview

The importGeoJSON method returns item collections. Don’t instantiate them directly.

## Topics

### Item collection properties

data

The raw GeoJSON data.

getFlattenedItemList

A flattened array of items that includes annotations and overlays.

items

A nested list of annotations, overlays, and other item collections.

## See Also

### Geographical features

importGeoJSON

Converts imported GeoJSON data to MapKit JS items.

GeoJSONDelegate

A delegate object that controls a GeoJSON import to override default behavior and provide custom style.

Displaying Indoor Maps with MapKit JS

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest in your browser.

