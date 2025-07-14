

- PencilKit
- PKInkingToolReference
-  init(ink:width:) 

Initializer

# init(ink:width:)

Create an inking tool with the specified ink and width.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
convenience init(
    ink: PKInk,
    width: CGFloat
)
```

## Parameters 

`ink`  

The shape of the tool. You may specify PKInkTypeMarker, PKInkTypePen, or PKInkTypePencil.

`width`  

The width of a line drawn with the tool.

## See Also

### Creating an inking tool

init(inkType: __PKInkType, color: UIColor, width: CGFloat)

Creates an ink tool object with the specified color and line width values.

convenience init(inkType: __PKInkType, color: UIColor)

Creates an ink tool object with the default line width and the specified color.

