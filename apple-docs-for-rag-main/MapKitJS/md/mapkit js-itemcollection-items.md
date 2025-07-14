

- MapKit JS
- ItemCollection
-  items 

Instance Property

# items

A nested list of annotations, overlays, and other item collections.

MapKit JS 5.0+

``` source
attribute (mapkit.Annotation|mapkit.Overlay|ItemCollection)[] items;
```

## Discussion

Access the original GeoJSON data in the data object. To retrieve the data as MapKit JS items, use the items or getFlattenedItemList objects.

## See Also

### Item collection properties

data

The raw GeoJSON data.

getFlattenedItemList

A flattened array of items that includes annotations and overlays.

