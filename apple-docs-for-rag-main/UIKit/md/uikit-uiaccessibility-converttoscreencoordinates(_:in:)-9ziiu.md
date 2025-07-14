

- UIKit
- UIAccessibility
-  convertToScreenCoordinates(\_:in:) 

Type Method

# convertToScreenCoordinates(\_:in:)

Converts the specified rectangle from view coordinates to screen coordinates.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
static func convertToScreenCoordinates(
    _ rect: CGRect,
    in view: UIView
) -> CGRect
```

## Parameters 

`rect`  

A rectangle specified in the coordinate system of the specified `view`.

`view`  

The view that contains the specified rectangle. This parameter must not be `nil`.

## Return Value

The rectangle in screen coordinates.

## Discussion

Use this function to convert accessibility frame rectangles to screen coordinates.

## See Also

### Conversions

static func convertToScreenCoordinates(UIBezierPath, in: UIView) -> UIBezierPath

Converts the specified path object to screen coordinates and returns a new path object with the results.

