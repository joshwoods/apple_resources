

- MapKit JS
- ItemCollection
-  getFlattenedItemList 

Instance Property

# getFlattenedItemList

A flattened array of items that includes annotations and overlays.

MapKit JS 5.0+

``` source
attribute (mapkit.Annotation|mapkit.Overlay)[] getFlattenedItemList;
```

## Discussion

The items in an ItemCollection may include nested item collections. Use getFlattenedItemList when you need a flat array that contains individual annotations and overlays.

Access the original GeoJSON data in the data object. To retrieve the data as MapKit JS items, use the items or getFlattenedItemList objects.

## See Also

### Item collection properties

data

The raw GeoJSON data.

items

A nested list of annotations, overlays, and other item collections.

