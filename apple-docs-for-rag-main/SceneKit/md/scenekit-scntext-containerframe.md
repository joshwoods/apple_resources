

- SceneKit
- SCNText
-  containerFrame 

Instance Property

# containerFrame

A rectangle specifying the area in which SceneKit should lay out the text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var containerFrame: CGRect { get set }
```

## Discussion

SceneKit can lay out a body of text to fit within a rectangular area. To do this, you must first use this property to define the area for text layout as a rectangle in the x- and y-axis dimensions of the text object’s local coordinate system. Then you use the isWrapped, alignmentMode, and truncationMode properties to control how SceneKit fits the text into the container frame. Text layout begins in the upper left corner of the rectangle.

The default value of this property is CGRectZero, specifying that SceneKit should lay out the text on one line without wrapping or truncation.

Depending on the content and style of the text and the values of the isWrapped, alignmentMode, and truncationMode properties, the text may not fit within the container frame after layout, or it may occupy a smaller area.

## See Also

### Managing Text Layout

var isWrapped: Bool

A Boolean value that specifies whether SceneKit wraps long lines of text.

var alignmentMode: String

A constant that specifies how SceneKit horizontally aligns each line of text within its container.

var truncationMode: String

A constant that specifies how SceneKit truncates text that is too long to fit its container.

var textSize: CGSize

The two-dimensional extent of the text after layout.

