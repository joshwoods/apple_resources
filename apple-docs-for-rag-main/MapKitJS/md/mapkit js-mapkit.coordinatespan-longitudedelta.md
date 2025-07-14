

- MapKit JS
- mapkit.CoordinateSpan
-  longitudeDelta 

Instance Property

# longitudeDelta

The amount of east-to-west distance (in degrees) to display for the map region.

MapKit JS 5.0+

``` source
attribute number longitudeDelta;
```

## Discussion

The number of kilometers spanned by a longitude range varies based on the current latitude. For example, one degree of longitude spans a distance of approximately 111 kilometers (69 miles) at the equator but shrinks to 0 kilometers at the poles.

## See Also

### Defining the span

latitudeDelta

The amount of north-to-south distance (in degrees) to display for the map region.

