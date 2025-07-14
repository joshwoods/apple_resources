

- Core Location
-  CLLocationCoordinate2DIsValid(\_:) 

Function

# CLLocationCoordinate2DIsValid(\_:)

Returns a Boolean value indicating whether the specified coordinate is valid.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CLLocationCoordinate2DIsValid(_ coord: CLLocationCoordinate2D) -> Bool
```

## Parameters 

`coord`  

A coordinate containing latitude and longitude values.

## Return Value

true if the coordinate is valid or false if it is not.

## Discussion

A coordinate is considered invalid if it meets at least one of the following criteria:

- Its latitude is greater than 90 degrees or less than -90 degrees.

- Its longitude is greater than 180 degrees or less than -180 degrees.

## See Also

### Validating a coordinate

let kCLLocationCoordinate2DInvalid: CLLocationCoordinate2D

An invalid coordinate value.

