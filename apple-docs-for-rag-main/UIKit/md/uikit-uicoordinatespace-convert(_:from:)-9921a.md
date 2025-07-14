

- UIKit
- UICoordinateSpace
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a rectangle from the specified coordinate space to the coordinate space of the current object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func convert(
    _ rect: CGRect,
    from coordinateSpace: any UICoordinateSpace
) -> CGRect
```

**Required**

## Parameters 

`rect`  

A rectangle in the specified coordinate space.

`coordinateSpace`  

The coordinate space in which `rect` is specified.

## Return Value

A rectangle specified in the coordinate space of the current object.

## See Also

### Converting between coordinate spaces

func convert(CGPoint, to: any UICoordinateSpace) -> CGPoint

Converts a point from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGPoint, from: any UICoordinateSpace) -> CGPoint

Converts a point from the specified coordinate space to the coordinate space of the current object.

**Required**

func convert(CGRect, to: any UICoordinateSpace) -> CGRect

Converts a rectangle from the coordinate space of the current object to the specified coordinate space.

**Required**

