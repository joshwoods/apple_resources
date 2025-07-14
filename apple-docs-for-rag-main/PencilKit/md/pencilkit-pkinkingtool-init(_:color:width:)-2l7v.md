

- PencilKit
- PKInkingTool
-  init(\_:color:width:) 

Initializer

# init(\_:color:width:)

Creates an ink tool object with the specified color and line width values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
init(
    _ inkType: PKInkingTool.InkType,
    color: UIColor = UIColor.black,
    width: CGFloat? = nil
)
```

## Parameters 

`inkType`  

The shape of the tool, which can be PKInkingTool.InkType.marker, PKInkingTool.InkType.pen, or PKInkingTool.InkType.pencil.

`color`  

The color to apply to drawn lines.

`width`  

The base width to apply to any drawn lines. The value in the `inkType` parameter and input from Apple Pencil affects the final width.

## Discussion

This initializer creates a new inking tool with the specified type, color, and width.

## See Also

### Creating an inking tool

init(PKInkingTool.InkType, color: NSColor, width: CGFloat?)

Creates an ink tool object with the specified color and line width values.

init(ink: PKInk, width: CGFloat)

Create an inking tool with the specified ink and width.

