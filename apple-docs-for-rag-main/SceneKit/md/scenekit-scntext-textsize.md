

- SceneKit
- SCNText
-  textSize 

Instance Property

# textSize

The two-dimensional extent of the text after layout.

macOS

``` source
var textSize: CGSize { get }
```

## Discussion

This property reports the size of the smallest bounding rectangle containing the text.

This size does not necessarily match that of the layout rectangle specified by the containerFrame property. A long body of text may overflow the layout rectangle, depending on the values of the isWrapped and truncationMode properties, and a short string of text may fit in an area smaller than the layout rectangle.

## See Also

### Managing Text Layout

var containerFrame: CGRect

A rectangle specifying the area in which SceneKit should lay out the text.

var isWrapped: Bool

A Boolean value that specifies whether SceneKit wraps long lines of text.

var alignmentMode: String

A constant that specifies how SceneKit horizontally aligns each line of text within its container.

var truncationMode: String

A constant that specifies how SceneKit truncates text that is too long to fit its container.

