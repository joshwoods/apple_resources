

- MapKit JS
-  mapkit.Map 

Class

# mapkit.Map

An embeddable interactive map that you add to a webpage.

MapKit JS 5.0+

``` source
interface mapkit.Map
```

## Mentioned in 

Adding interactivity to overlays

## Overview

A map is a self-contained view object that you embed on a webpage. It’s possible to have multiple independent maps on a single webpage, although typically webpages only need one interactive map.

## Topics

### Creating a map

mapkit.Map

Creates a map you embed on a webpage and initializes it with the constructor options you choose.

MapConstructorOptions

An object that contains options for creating a map’s features.

### Handling map events

Handling map events

Register an event lister for events that a map object dispatches.

addEventListener

Adds an event listener to handle events that user interactions and the framework trigger.

removeEventListener

Removes an event listener.

### Accessing interaction properties

isRotationAvailable

A Boolean value that indicates whether map rotation is available.

isRotationEnabled

A Boolean value that determines whether the user may rotate the map using the compass control or a rotate gesture.

isScrollEnabled

A Boolean value that determines whether the user can cause the map to scroll with a pointing device or with gestures on a touchscreen.

isZoomEnabled

A Boolean value that determines whether the user may zoom in and out on the map using pinch gestures or the zoom control.

### Manipulating the visible portion of the map

center

The map coordinate at the center of the map view.

setCenterAnimated

Centers the map to the provided coordinate, with optional animation.

region

The area the map is displaying.

setRegionAnimated

Changes the map’s region to the provided region, with optional animation.

rotation

The map’s rotation, in degrees.

setRotationAnimated

Changes the map’s rotation setting to the number of specified degrees.

visibleMapRect

The visible area of the map, in map units.

setVisibleMapRectAnimated

Changes the map’s visible map rectangle to the specified map rectangle.

cameraBoundary

A constraint of the location of the center of the map.

setCameraBoundaryAnimated

Changes the map’s camera boundary with an animated transition.

cameraDistance

The altitude of the camera relative to the elevation of the center of the map.

setCameraDistanceAnimated

Changes the map’s camera distance with an animated transition.

cameraZoomRange

The minimum and maximum distances of the camera from the map center.

setCameraZoomRangeAnimated

Changes the map’s camera zoom range with an animated transition.

### Showing the map’s controls

showsCompass

A feature visibility setting that determines when the compass is visible.

showsMapTypeControl

A Boolean value that determines whether to display a control that lets users choose the map type.

showsScale

A feature visibility setting that determines when the map displays the map’s scale indicator.

showsUserLocationControl

A Boolean value that determines whether the user location control is visible.

showsZoomControl

A Boolean value that determines whether to display a control for zooming in and zooming out on a map.

### Configuring the map’s appearance

colorScheme

The map’s color scheme when displaying standard or muted standard map types.

mapkit.Map.ColorSchemes

Constants indicating the color scheme of the map.

distances

The system of measurement that displays on the map.

mapkit.Map.Distances

Constants indicating the system of measurement that displays on the map.

mapType

The type of data that the map displays.

mapkit.Map.MapTypes

Constants representing the type of map to display.

padding

The map’s inset margins.

pointOfInterestFilter

The filter that determines the points of interest that display on the map.

showsPointsOfInterest

A Boolean value that determines whether the map displays points of interest.

showItems

Adjusts the map’s visible region to bring the specified overlays and annotations into view.

MapShowItemsOptions

Options that determine the map parameters to use when showing items.

tintColor

The CSS color that MapKit JS uses for user interface controls on the map.

### Annotating the map

annotations

An array of all the annotations on the map.

selectedAnnotation

The selected annotation.

annotationForCluster

A delegate method for modifying an annotation that represents a group of annotations that the framework combines into a cluster.

annotationsInMapRect

Returns the list of annotation objects within the specified map rectangle.

addAnnotation

Adds an annotation to the map.

addAnnotations

Adds an array of annotations to the map.

removeAnnotation

Removes an annotation from the map.

removeAnnotations

Removes multiple annotations from the map.

### Adding and removing overlays

overlays

An array of all of the map’s overlays.

selectedOverlay

The selected overlay on the map.

overlaysAtPoint

Returns an array of overlays at a given point on the webpage.

addOverlay

Adds an overlay to the map.

addOverlays

Adds multiple overlays to the map.

removeOverlay

Removes an overlay from the map.

removeOverlays

Removes multiple overlays from the map.

topOverlayAtPoint

Returns the topmost overlay at a given point on the webpage.

### Adding and removing geographical features

addItems

Adds a collection of annotations, overlays, or other item collections to the map.

removeItems

Removes a collection of annotations, overlays, or other item collections from the map.

### Adding and removing tile overlays

tileOverlays

An array of all of the map’s tile overlays.

addTileOverlay

Adds a tile overlay to the map.

addTileOverlays

Adds an array of tile overlays to the map.

removeTileOverlay

Removes a tile overlay from the map.

removeTileOverlays

Removes an array of tile overlays from the map.

### Displaying the user’s location

showsUserLocation

A Boolean value that determines whether to show the user’s location on the map.

tracksUserLocation

A Boolean value that determines whether to center the map on the user’s location.

userLocationAnnotation

An annotation that indicates the user’s location on the map.

### Converting map coordinates

convertCoordinateToPointOnPage

Converts a coordinate on the map to a point in the page’s coordinate system.

convertPointOnPageToCoordinate

Converts a point in page coordinates to the corresponding map coordinate.

### Destroying a map

destroy

Removes the map’s element from the DOM and releases internal references to the map to free up memory.

### Accessing the element

element

The map’s DOM element.

### Selecting map features

selectableMapFeatures

An array of map features that users can select from the map.

selectableMapFeatureSelectionAccessory

An accessory for displaying place information when a person selects a map feature.

annotationForMapFeature

The method MapKit JS calls when the framework creates a map feature annotation.

### Prioritizing feature loading

loadPriority

A value MapKit JS uses for prioritizing the visibility of specific map features before the underlaying map tiles.

mapkit.Map.LoadPriorities

Values for prioritizing the visibility of specific map features while the map is loading.

## See Also

### Maps

maps

An array that automatically adds and removes maps as the framework creates and destroys them.

