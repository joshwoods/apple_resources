

- Core Graphics
- CGContext
-  convertToDeviceSpace(\_:) 

Instance Method

# convertToDeviceSpace(\_:)

Returns a point that is transformed from user space coordinates to device space coordinates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func convertToDeviceSpace(_ point: CGPoint) -> CGPoint
```

## Parameters 

`point`  

The point, in user space coordinates, to transform.

## Return Value

The coordinates of the point in device space coordinates.

## See Also

### Converting Between Coordinate Spaces

var userSpaceToDeviceSpaceTransform: CGAffineTransform

Returns an affine transform that maps user space coordinates to device space coordinates.

func convertToUserSpace(CGPoint) -> CGPoint

Returns a point that is transformed from device space coordinates to user space coordinates.

func convertToDeviceSpace(CGRect) -> CGRect

Returns a rectangle that is transformed from user space coordinate to device space coordinates.

func convertToUserSpace(CGRect) -> CGRect

Returns a rectangle that is transformed from device space coordinate to user space coordinates.

func convertToDeviceSpace(CGSize) -> CGSize

Returns a size that is transformed from user space coordinates to device space coordinates.

func convertToUserSpace(CGSize) -> CGSize

Returns a size that is transformed from device space coordinates to user space coordinates.

