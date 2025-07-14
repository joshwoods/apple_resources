

- PencilKit
- PKInk
-  init(\_:color:) 

Initializer

# init(\_:color:)

Creates a new ink, specifying its type and color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    _ inkType: PKInk.InkType,
    color: UIColor = UIColor.black
)
```

## Parameters 

`inkType`  

The type of ink represented by one of the available PKInkingTool.InkType enumerations.

`color`  

The color of the ink; the default is black.

## See Also

### Creating an ink object

init(PKInk.InkType, color: NSColor)

Creates a new ink, specifying its type and color.

typealias InkType

A type alias referring to the ink type of an inking tool.

