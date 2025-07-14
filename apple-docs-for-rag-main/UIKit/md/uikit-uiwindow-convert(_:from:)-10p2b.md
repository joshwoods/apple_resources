

- UIKit
- UIWindow
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a rectangle from the coordinate system of another window to coordinate system of the current window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func convert(
    _ rect: CGRect,
    from window: UIWindow?
) -> CGRect
```

## Parameters 

`rect`  

A rectangle in the coordinate system of `window`.

`window`  

The source window containing the specified `rect`. Specify `nil` to convert the rectangle from the logical coordinate system of the screen, which is measured in points.

## Return Value

The converted rectangle.

## See Also

### Converting coordinates

func convert(CGPoint, to: UIWindow?) -> CGPoint

Converts a point from the current window’s coordinate system to the coordinate system of another window.

func convert(CGPoint, from: UIWindow?) -> CGPoint

Converts a point from the coordinate system of a given window to the coordinate system of the current window.

func convert(CGRect, to: UIWindow?) -> CGRect

Converts a rectangle from the current window’s coordinate system to the coordinate system of another window.

