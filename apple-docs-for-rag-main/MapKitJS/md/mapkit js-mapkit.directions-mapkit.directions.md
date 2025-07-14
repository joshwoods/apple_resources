

- MapKit JS
- mapkit.Directions
-  mapkit.Directions 

Initializer

# mapkit.Directions

Creates a directions object with options you provide.

MapKit JS 5.0+

``` source
new mapkit.Directions(
 optional DirectionsConstructorOptions options
);
```

## Parameters 

`options`  

An object containing the options for creating a directions object. This parameter is optional.

## Discussion

To request directions, create an instance of the mapkit.Directions object, then call the route function with a DirectionsRequest object as the first parameter. The second parameter for route is a callback function, through which MapKit JS returns the directions response asynchronously.

To return directions in a specific language, set language in DirectionsConstructorOptions when you create an instance of the mapkit.Directions object.

## See Also

### Creating a directions object

DirectionsConstructorOptions

Options that you may provide when creating a directions object.

