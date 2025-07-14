

- MapKit JS
- mapkit.Map
-  padding 

Instance Property

# padding

The map’s inset margins.

MapKit JS 5.0+

``` source
attribute mapkit.Padding padding;
```

## Mentioned in 

MapKit JS 5

## Discussion

The padding affects the map’s controls layout. The map computes the region it draws to fit within the inset frame that the padding specifies.

MapKit JS computes the visibleMapRect to fit within the inset frame with the constraint that the entire, noninset frame needs to be able to contain map data as well. Using the showItems method ensures that all annotations and overlays are visible within the inset frame. The map modifies the region when displaying an annotation’s callout to ensure it’s entirely visible within the inset frame.

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

