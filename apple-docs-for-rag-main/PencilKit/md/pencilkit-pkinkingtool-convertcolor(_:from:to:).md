

- PencilKit
- PKInkingTool
-  convertColor(\_:from:to:) 

Type Method

# convertColor(\_:from:to:)

Convert a color from one user interface style to another.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
static func convertColor(
    _ color: UIColor,
    from: UIUserInterfaceStyle,
    to: UIUserInterfaceStyle
) -> UIColor
```

## Parameters 

`color`  

The color to convert.

`from`  

The user interface style to convert the color from.

`to`  

The user interface style to convert the color to.

## Return Value

A UIColor from the user interface style specified in the `to` parameter.

