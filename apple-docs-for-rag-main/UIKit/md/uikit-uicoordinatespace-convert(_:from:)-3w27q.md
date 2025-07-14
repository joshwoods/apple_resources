

- UIKit
- UICoordinateSpace
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a point from the specified coordinate space to the coordinate space of the current object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func convert(
    _ point: CGPoint,
    from coordinateSpace: any UICoordinateSpace
) -> CGPoint
```

**Required**

## Parameters 

`point`  

A point in the specified coordinate space.

`coordinateSpace`  

The coordinate space in which `point` is specified.

## Return Value

A point specified in the coordinate space of the current object.

## See Also

### Converting between coordinate spaces

func convert(CGPoint, to: any UICoordinateSpace) -> CGPoint

Converts a point from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGRect, to: any UICoordinateSpace) -> CGRect

Converts a rectangle from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGRect, from: any UICoordinateSpace) -> CGRect

Converts a rectangle from the specified coordinate space to the coordinate space of the current object.

**Required**

