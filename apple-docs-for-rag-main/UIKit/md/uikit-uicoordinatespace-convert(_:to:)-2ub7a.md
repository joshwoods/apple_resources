

- UIKit
- UICoordinateSpace
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a point from the coordinate space of the current object to the specified coordinate space.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func convert(
    _ point: CGPoint,
    to coordinateSpace: any UICoordinateSpace
) -> CGPoint
```

**Required**

## Parameters 

`point`  

A point specified in the coordinate system of the current object.

`coordinateSpace`  

The coordinate space into which `point` is to be converted.

## Return Value

A point specified in the target coordinate space.

## See Also

### Converting between coordinate spaces

func convert(CGPoint, from: any UICoordinateSpace) -> CGPoint

Converts a point from the specified coordinate space to the coordinate space of the current object.

**Required**

func convert(CGRect, to: any UICoordinateSpace) -> CGRect

Converts a rectangle from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGRect, from: any UICoordinateSpace) -> CGRect

Converts a rectangle from the specified coordinate space to the coordinate space of the current object.

**Required**

