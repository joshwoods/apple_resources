

- PencilKit
- PKInkingToolReference
-  init(inkType:color:) 

Initializer

# init(inkType:color:)

Creates an ink tool object with the default line width and the specified color.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
convenience init(
    inkType type: __PKInkType,
    color: UIColor
)
```

**macOS**

``` source
convenience init(
    inkType type: __PKInkType,
    color: NSColor
)
```

## Parameters 

`type`  

The shape of the tool. You may specify PKInkTypeMarker, PKInkTypePen, or PKInkTypePencil.

`color`  

The color to apply to drawn lines.

## Return Value

A new inking tool with the specified type and color.

## Discussion

This method sets the line width to the value returned by defaultWidth(forInkType:).

## See Also

### Creating an inking tool

init(inkType: __PKInkType, color: UIColor, width: CGFloat)

Creates an ink tool object with the specified color and line width values.

convenience init(ink: PKInk, width: CGFloat)

Create an inking tool with the specified ink and width.

