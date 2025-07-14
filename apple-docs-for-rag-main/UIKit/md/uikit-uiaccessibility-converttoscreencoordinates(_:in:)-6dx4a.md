

- UIKit
- UIAccessibility
-  convertToScreenCoordinates(\_:in:) 

Type Method

# convertToScreenCoordinates(\_:in:)

Converts the specified path object to screen coordinates and returns a new path object with the results.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
static func convertToScreenCoordinates(
    _ path: UIBezierPath,
    in view: UIView
) -> UIBezierPath
```

## Parameters 

`path`  

The path object that you want to convert. The coordinate values used to create this path object should be relative to the coordinate system of the specified `view`. This parameter must not be `nil`.

`view`  

The view whose coordinate system was used to define the path. This parameter must not be `nil`.

## Return Value

A new path object that has the same shape as `path` but whose points are specified in screen coordinates.

## Discussion

This function adjusts the points of the path you provide to values that the accessibility system can use. You can use it to convert path objects in use by your app’s user interface before handing them to the accessibility system.

## See Also

### Conversions

static func convertToScreenCoordinates(CGRect, in: UIView) -> CGRect

Converts the specified rectangle from view coordinates to screen coordinates.

