

- PencilKit
- PKInkReference
-  init(inkType:color:) 

Initializer

# init(inkType:color:)

Create a new ink, specifying its type, color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

**macOS**

``` source
init(
    inkType type: __PKInkType,
    color: NSColor
)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
init(
    inkType type: __PKInkType,
    color: UIColor
)
```

## Parameters 

`type`  

The type of ink to create, from one of the available PKInkType enumerations.

`color`  

The base color for this ink.

