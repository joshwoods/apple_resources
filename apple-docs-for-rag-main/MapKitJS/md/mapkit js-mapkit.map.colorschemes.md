

- MapKit JS
-  mapkit.Map.ColorSchemes 

Enumeration

# mapkit.Map.ColorSchemes

Constants indicating the color scheme of the map.

MapKit JS 5.12+

``` source
interface mapkit.Map.ColorSchemes {
 const string Light;
 const string Dark;
 const string Adaptive;
};
```

## Overview

Color schemes apply to maps that have a standard or muted standard map type (Standard or MutedStandard). Use these constants with the map’s colorScheme property.

## Topics

### Color scheme values

Adaptive

A constant indicating a color scheme that follows the current system setting.

Light

A constant indicating a light color scheme.

Dark

A constant indicating a dark color scheme.

## See Also

### Configuring the map’s appearance

colorScheme

The map’s color scheme when displaying standard or muted standard map types.

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

