

- PencilKit
- PKInkingToolReference
-  init(inkType:color:width:) 

Initializer

# init(inkType:color:width:)

Creates an ink tool object with the specified color and line width values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

**macOS**

``` source
init(
    inkType type: __PKInkType,
    color: NSColor,
    width: CGFloat
)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
init(
    inkType type: __PKInkType,
    color: UIColor,
    width: CGFloat
)
```

## Parameters 

`type`  

The shape of the tool. You may specify PKInkTypeMarker, PKInkTypePen, or PKInkTypePencil.

`color`  

The color to apply to drawn lines.

`width`  

The base width to apply to any drawn lines. The value in the `inkType` parameter and input from Apple Pencil affects the final actual width.

## Return Value

A new inking tool with the specified type, color, and width.

## See Also

### Creating an inking tool

convenience init(inkType: __PKInkType, color: UIColor)

Creates an ink tool object with the default line width and the specified color.

convenience init(ink: PKInk, width: CGFloat)

Create an inking tool with the specified ink and width.

