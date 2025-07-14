

- MapKit JS
-  MapConstructorOptions 

Class

# MapConstructorOptions

An object that contains options for creating a map’s features.

MapKit JS 5.0+

``` source
interface MapConstructorOptions
```

## Overview

Use MapConstructorOptions to set the initial characteristics for your map, including the visible portion of the map, which controls are visible, the configuration of overlays and annotations, and the visibility of the user’s location.

## Topics

### Controlling the visible portion of the map

visibleMapRect

The visible area of the map, in map units.

region

The area the map is displaying.

center

The map coordinate at the center of the map view.

rotation

The map’s rotation, in degrees.

tintColor

The CSS color that MapKit JS uses for the user interface controls on the map.

### Setting the map’s appearance and controls

colorScheme

The map’s color scheme when displaying standard or muted standard map types.

mapType

The type of data that the map view displays.

padding

The map’s inset margins.

showsMapTypeControl

A Boolean value that determines whether to display a control that lets users choose the map type.

isRotationEnabled

A Boolean value that determines whether the user may rotate the map using the compass control or a rotate gesture.

showsCompass

A feature visibility setting that determines when the compass is visible.

isZoomEnabled

A Boolean value that determines whether the user may zoom in and out on the map using pinch gestures or the zoom control.

showsZoomControl

A Boolean value that determines whether to display a control for zooming in and zooming out on a map.

isScrollEnabled

A Boolean value that determines whether the user may scroll the map with a pointing device or gestures on a touchscreen.

showsScale

A feature visibility setting that allows you to determine when to display the map’s scale.

### Configuring map annotations

annotationForCluster

Modifies cluster annotations.

annotations

An array holding all the annotations on the map.

selectedAnnotation

The selected annotation on the map.

### Configuring map overlays

overlays

An array that contains all of the map’s overlays.

selectedOverlay

The selected overlay on the map.

showsPointsOfInterest

A Boolean value that determines whether the map displays points of interest.

pointOfInterestFilter

The filter that determines the points of interest that display on the map.

### Enabling user location

showsUserLocation

A Boolean value that determines whether to show the user’s location on the map.

tracksUserLocation

A Boolean value that determines whether to center the map on the user’s location.

showsUserLocationControl

A Boolean value that determines whether the user location control is visible.

### Setting the loading priority

loadPriority

A value MapKit JS uses for prioritizing the visibility of specific map features before the underlaying map tiles.

mapkit.Map.LoadPriorities

Values for prioritizing the visibility of specific map features while the map is loading.

## See Also

### Creating a map

mapkit.Map

Creates a map you embed on a webpage and initializes it with the constructor options you choose.

