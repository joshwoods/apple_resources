

- Core Location
-  CLLocationCoordinate2DMake(\_:\_:) 

Function

# CLLocationCoordinate2DMake(\_:\_:)

Formats a latitude and longitude value into a coordinate data structure format.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CLLocationCoordinate2DMake(
    _ latitude: CLLocationDegrees,
    _ longitude: CLLocationDegrees
) -> CLLocationCoordinate2D
```

## Parameters 

`latitude`  

The latitude for the new coordinate.

`longitude`  

The longitude for the new coordinate.

## Return Value

A coordinate structure encompassing the latitude and longitude values.

## See Also

### Creating a location coordinate

init()

Creates a location coordinate object.

init(latitude: CLLocationDegrees, longitude: CLLocationDegrees)

Creates a location coordination object with the specified latitude and longitude values.

