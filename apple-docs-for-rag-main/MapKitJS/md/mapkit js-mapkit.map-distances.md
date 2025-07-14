

- MapKit JS
- mapkit.Map
-  distances 

Instance Property

# distances

The system of measurement that displays on the map.

MapKit JS 5.12+

``` source
attribute string distances;
```

## Mentioned in 

MapKit JS 5

## Discussion

Sets the system of measurement for displaying map distances. See mapkit.Map.Distances for accepted values.

This property applies to the scale, if it displays. The default value is Adaptive, which means that the measurement system depends on the map’s set language. This property affects displayed distances only; it doesn’t affect data that returns from a service, such as mapkit.Directions.

## Topics

### Distances

mapkit.Map.Distances

Constants indicating the system of measurement that displays on the map.

## See Also

### Configuring the map’s appearance

colorScheme

The map’s color scheme when displaying standard or muted standard map types.

mapkit.Map.ColorSchemes

Constants indicating the color scheme of the map.

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

