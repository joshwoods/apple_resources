

- MapKit JS
-  MapShowItemsOptions 

Structure

# MapShowItemsOptions

Options that determine the map parameters to use when showing items.

MapKit JS 5.0+

``` source
dictionary MapShowItemsOptions {
 boolean animate;
 mapkit.Padding padding;
 mapkit.CoordinateSpan minimumSpan;
};
```

## Overview

Use these options when calling showItems.

## Topics

### Show item options

animate

A Boolean value that determines whether the map animates as the map region changes to show the items.

minimumSpan

The minimum longitudinal and latitudinal span the map displays.

padding

Spacing that the framework adds around the computed map region when showing items.

## See Also

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

tintColor

The CSS color that MapKit JS uses for user interface controls on the map.

