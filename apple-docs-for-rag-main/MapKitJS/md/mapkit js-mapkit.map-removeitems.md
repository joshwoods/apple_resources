

- MapKit JS
- mapkit.Map
-  removeItems 

Instance Method

# removeItems

Removes a collection of annotations, overlays, or other item collections from the map.

MapKit JS 5.0+

``` source
(mapkit.Annotation|mapkit.Overlay|ItemCollection)[]|ItemCollection removeItems();
```

## Parameters 

`items`  

An array of annotations, overlays, or the data returned from importGeoJSON to display on the map.

## Return Value

Returns an array of items removed from the map.

## Discussion

This method doesn’t change the map’s visible region. Use showItems with a list of items to focus on to update the map’s view.

## See Also

### Adding and removing geographical features

addItems

Adds a collection of annotations, overlays, or other item collections to the map.

