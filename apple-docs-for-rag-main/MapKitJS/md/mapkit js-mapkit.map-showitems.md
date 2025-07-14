

- MapKit JS
- mapkit.Map
-  showItems 

Instance Method

# showItems

Adjusts the map’s visible region to bring the specified overlays and annotations into view.

MapKit JS 5.0+

``` source
(mapkit.Annotation|mapkit.Overlay|ItemCollection)[] showItems();
```

## Parameters 

`items`  

An array of annotations and overlays to make visible.

`options`  

Options that MapShowItemsOptions defines that let you determine animation, padding, and the minimum span of the map’s region.

## Return Value

Returns the items array that you pass.

## Mentioned in 

MapKit JS 5

## Discussion

The method showItems adjusts the map’s region to bring all of the specified items — annotations and overlays — into view. The system only adds items if they’re not already on the map.

The map’s adjusted region covers the smallest longitudinal span possible. For example, passing an array that consists of two annotations for the cities Tokyo and Los Angeles, and a polyline that represents the flight path between them, to showItems updates the region to cover the Pacific Ocean.

The showItems method factors in the size of the specified annotations when updating the map’s region so the entirety of the annotations are visible. Similarly, it ensures that the map shows an overlay with thick lines in its entirety. In some cases, it’s possible that the map can’t show all items at once, or the actual padding doesn’t match the requested padding. This happens if:

- One or more items falls outside of the visible map region, even at the minimum zoom level.

- The zoom level, which determines the amount of padding, snaps to a level that has a different amount of padding than you request.

This method throws an `Error` if the arguments to the method are invalid.

The following example demonstrates how to use `showItems:`

```
var park = new mapkit.MarkerAnnotation(new mapkit.Coordinate(37.749581, -119.524212), { title: "Yosemite" }),
    surf = new mapkit.MarkerAnnotation(new mapkit.Coordinate(37.49557, -122.496687), { title: "Mavericks" });
map.showItems([park, surf],
              { animate: true,
                padding: new mapkit.Padding(60, 25, 60, 25)
              });  
```

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

MapShowItemsOptions

Options that determine the map parameters to use when showing items.

tintColor

The CSS color that MapKit JS uses for user interface controls on the map.

