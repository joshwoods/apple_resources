

- MapKit
- MKMultiPoint
-  getCoordinates(\_:range:) 

Instance Method

# getCoordinates(\_:range:)

Retrieves one or more points associated with the shape and converts them to coordinate values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func getCoordinates(
    _ coords: UnsafeMutablePointer,
    range: NSRange
)
```

## Parameters 

`coords`  

On input, provide a C array of structures large enough to hold the desired number of coordinates. On output, this structure contains the requested coordinate data.

`range`  

The range of points you want. The `location` field indicates the first point you’re requesting, with `0` being the first point, `1` being the second point, and so on. The `length` field indicates the number of points you want. The array in `coords` needs to be large enough to accommodate the number of requested coordinates.

## Discussion

This method converts the map points into coordinates before returning them to you. If you want to specify the value of each point as a map point, you can access the values directly using the points() method.

