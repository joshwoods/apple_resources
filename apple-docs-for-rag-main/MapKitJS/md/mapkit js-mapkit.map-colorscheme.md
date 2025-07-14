

- MapKit JS
- mapkit.Map
-  colorScheme 

Instance Property

# colorScheme

The map’s color scheme when displaying standard or muted standard map types.

MapKit JS 5.12+

``` source
attribute string colorScheme;
```

## Mentioned in 

MapKit JS 5

## Discussion

This property accepts a property from mapkit.Map.ColorSchemes to determine whether the map displays with a dark or light theme when Standard or MutedStandard are the configured mapType. The default is Light.

The grid, user location accuracy ring, labels for marker annotations, and controls of the map change appearance to complement the Dark Mode style.

## Topics

### Color Schemes

mapkit.Map.ColorSchemes

Constants indicating the color scheme of the map.

## See Also

### Configuring the map’s appearance

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

