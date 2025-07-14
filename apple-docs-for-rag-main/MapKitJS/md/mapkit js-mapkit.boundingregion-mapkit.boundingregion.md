

- MapKit JS
- mapkit.BoundingRegion
-  mapkit.BoundingRegion 

Initializer

# mapkit.BoundingRegion

Creates a rectangular bounding region, which the latitude and longitude coordinates of the rectangle’s northeast and southwest corners define.

MapKit JS 5.0+

``` source
new mapkit.BoundingRegion(
 number northLatitude,
 number eastLongitude,
 number southLatitude,
 number westLongitude
);
```

## Parameters 

`northLatitude`  

The north latitude of the bounding region.

`eastLongitude`  

The east longitude of the bounding region.

`southLatitude`  

The south latitude of the bounding region.

`westLongitude`  

The west longitude of the bounding region.

## Discussion

The example below creates a new bounding region by passing the required longitude and latitude coordinates to the constructor:

```
```

