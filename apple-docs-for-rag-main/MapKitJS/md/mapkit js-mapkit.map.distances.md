

- MapKit JS
-  mapkit.Map.Distances 

Enumeration

# mapkit.Map.Distances

Constants indicating the system of measurement that displays on the map.

MapKit JS 5.12+

``` source
interface mapkit.Map.Distances {
 const string Metric;
 const string Imperial;
 const string Adaptive;
};
```

## Overview

Use these constants with the map’s distances property.

## Topics

### Distances Values

Adaptive

A constant indicating the measurement system is adaptive, and determined based on the map’s language.

Metric

A constant indicating the measurement system is metric.

Imperial

A constant indicating the measurement system is imperial.

## See Also

### Configuring the map’s appearance

colorScheme

The map’s color scheme when displaying standard or muted standard map types.

mapkit.Map.ColorSchemes

Constants indicating the color scheme of the map.

distances

The system of measurement that displays on the map.

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

