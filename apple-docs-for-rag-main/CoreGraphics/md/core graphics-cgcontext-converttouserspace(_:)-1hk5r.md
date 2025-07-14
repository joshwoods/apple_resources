

- Core Graphics
- CGContext
-  convertToUserSpace(\_:) 

Instance Method

# convertToUserSpace(\_:)

Returns a rectangle that is transformed from device space coordinate to user space coordinates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func convertToUserSpace(_ rect: CGRect) -> CGRect
```

## Parameters 

`rect`  

The rectangle, in device space coordinates, to transform.

## Return Value

The rectangle in user space coordinates.

## Discussion

In general, affine transforms do not preserve rectangles. As a result, this function returns the smallest rectangle that contains the transformed corner points of the rectangle.

## See Also

### Converting Between Coordinate Spaces

var userSpaceToDeviceSpaceTransform: CGAffineTransform

Returns an affine transform that maps user space coordinates to device space coordinates.

func convertToDeviceSpace(CGPoint) -> CGPoint

Returns a point that is transformed from user space coordinates to device space coordinates.

func convertToUserSpace(CGPoint) -> CGPoint

Returns a point that is transformed from device space coordinates to user space coordinates.

func convertToDeviceSpace(CGRect) -> CGRect

Returns a rectangle that is transformed from user space coordinate to device space coordinates.

func convertToDeviceSpace(CGSize) -> CGSize

Returns a size that is transformed from user space coordinates to device space coordinates.

func convertToUserSpace(CGSize) -> CGSize

Returns a size that is transformed from device space coordinates to user space coordinates.

