

- UIKit
- UIWindow
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a rectangle from the current window’s coordinate system to the coordinate system of another window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func convert(
    _ rect: CGRect,
    to window: UIWindow?
) -> CGRect
```

## Parameters 

`rect`  

A rectangle in the current window’s coordinate system.

`window`  

The window defining the destination coordinate system for `rect`. Specify `nil` to convert the rectangle to the logical coordinate system of the screen, which is measured in points.

## Return Value

The rectangle converted to the coordinate system of `window`.

## See Also

### Converting coordinates

func convert(CGPoint, to: UIWindow?) -> CGPoint

Converts a point from the current window’s coordinate system to the coordinate system of another window.

func convert(CGPoint, from: UIWindow?) -> CGPoint

Converts a point from the coordinate system of a given window to the coordinate system of the current window.

func convert(CGRect, from: UIWindow?) -> CGRect

Converts a rectangle from the coordinate system of another window to coordinate system of the current window.

