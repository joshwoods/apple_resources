

- MapKit JS
- mapkit.Map
-  userLocationAnnotation 

Instance Property

# userLocationAnnotation

An annotation that indicates the user’s location on the map.

MapKit JS 5.0+

``` source
readonly attribute mapkit.Annotation userLocationAnnotation;
```

## Discussion

This is the annotation, or blue dot, that indicates the user’s location on the map. This property is `null` if:

- showsUserLocation is `false`

- MapKit JS is trying to acquire the user’s location

- MapKit JS fails to acquire the user’s location

The map’s annotations property only holds annotations you can modify. MapKit JS doesn’t add the userLocationAnnotation property to the annotations array, and you can’t remove it by using removeAnnotation. Use selectedAnnotation to reference the user’s location annotation when it’s in a selected state.

The default value of the collisionMode property on the user’s location annotation is None. The user’s location annotation doesn’t collide with other annotations unless you set the collision mode property to a value other than `None`.

## See Also

### Displaying the user’s location

showsUserLocation

A Boolean value that determines whether to show the user’s location on the map.

tracksUserLocation

A Boolean value that determines whether to center the map on the user’s location.

