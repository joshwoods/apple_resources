

- SceneKit
- SCNText
-  alignmentMode 

Instance Property

# alignmentMode

A constant that specifies how SceneKit horizontally aligns each line of text within its container.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var alignmentMode: String { get set }
```

## Discussion

When you define a layout rectangle for the text using its containerFrame property, SceneKit uses the alignmentMode property to determine where each line of text is placed horizontally relative to the layout rectangle. For possible values, see Horizontal alignment modes in CATextLayer.

The default value of this property is natural, specifying that text is aligned relative to the default alignment of its script. (For example, left-to-right languages are left-aligned.)

## See Also

### Managing Text Layout

var containerFrame: CGRect

A rectangle specifying the area in which SceneKit should lay out the text.

var isWrapped: Bool

A Boolean value that specifies whether SceneKit wraps long lines of text.

var truncationMode: String

A constant that specifies how SceneKit truncates text that is too long to fit its container.

var textSize: CGSize

The two-dimensional extent of the text after layout.

