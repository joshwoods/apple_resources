

- MapKit JS
- mapkit.Overlay
-  map 

Instance Property

# map

The map you add the overlay to.

MapKit JS 5.0+

``` source
readonly attribute mapkit.Map map;
```

## Discussion

This property is `null` if you don’t add the overlay to a map, or if you remove it from a map.

## See Also

### Setting overlay options

data

Custom data to associate with the overlay.

visible

A Boolean value that determines whether an overlay is visible.

enabled

A Boolean value that determines whether the overlay responds to user interaction.

selected

A Boolean value that indicates whether the user selects the overlay.

style

Style properties to apply to the overlay.

