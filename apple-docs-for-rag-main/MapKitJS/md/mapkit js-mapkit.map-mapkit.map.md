

- MapKit JS
- mapkit.Map
-  mapkit.Map 

Initializer

# mapkit.Map

Creates a map you embed on a webpage and initializes it with the constructor options you choose.

MapKit JS 5.0+

``` source
new mapkit.Map(
 optional string|Element parent,
 optional MapConstructorOptions options
);
```

## Parameters 

`parent`  

A DOM element, or the ID of a DOM element, to use as your map’s container.

`options`  

Options that MapConstructorOptions defines for initializing the properties of your map.

## Return Value

A mapkit.Map instance.

## Discussion

The map’s constructor takes an optional `parent` argument and an optional `options` argument. If you specify the `parent` argument, MapKit JS inserts the map element into the DOM as a descendant of `parent` that it styles to fill the size of its enclosing element. A map defaults to showing the entire world.

The following example demonstrates how to add a map to a `DIV` element using HTML:

```

```

The following example demonstrates how to add a map to a `DIV` element using JavaScript:

```
var map = new mapkit.Map('mapContainer', { center: new mapkit.Coordinate(37.334883, -122.008977) });
```

## See Also

### Creating a map

MapConstructorOptions

An object that contains options for creating a map’s features.

