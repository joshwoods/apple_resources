

- MapKit JS
- mapkit.Map
-  addItems 

Instance Method

# addItems

Adds a collection of annotations, overlays, or other item collections to the map.

MapKit JS 5.0+

``` source
(mapkit.Annotation|mapkit.Overlay|ItemCollection)[]|ItemCollection addItems();
```

## Parameters 

`items`  

An array of annotations, overlays, or the data returned from importGeoJSON to display on the map.

## Return Value

Returns an array of items added to the map.

## Mentioned in 

MapKit JS 5

## Discussion

Use addItems to add elements to the map after importing them from importGeoJSON.

This method doesn’t change the map’s visible region. Use showItems with the list of items to change the map’s view.

## See Also

### Adding and removing geographical features

removeItems

Removes a collection of annotations, overlays, or other item collections from the map.

