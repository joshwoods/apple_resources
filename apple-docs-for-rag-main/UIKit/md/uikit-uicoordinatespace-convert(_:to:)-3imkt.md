

- UIKit
- UICoordinateSpace
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a rectangle from the coordinate space of the current object to the specified coordinate space.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func convert(
    _ rect: CGRect,
    to coordinateSpace: any UICoordinateSpace
) -> CGRect
```

**Required**

## Parameters 

`rect`  

A rectangle specified in the coordinate system of the current object.

`coordinateSpace`  

The coordinate space into which `rect` is to be converted.

## Return Value

A rectangle specified in the target coordinate space.

## See Also

### Converting between coordinate spaces

func convert(CGPoint, to: any UICoordinateSpace) -> CGPoint

Converts a point from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGPoint, from: any UICoordinateSpace) -> CGPoint

Converts a point from the specified coordinate space to the coordinate space of the current object.

**Required**

func convert(CGRect, from: any UICoordinateSpace) -> CGRect

Converts a rectangle from the specified coordinate space to the coordinate space of the current object.

**Required**

