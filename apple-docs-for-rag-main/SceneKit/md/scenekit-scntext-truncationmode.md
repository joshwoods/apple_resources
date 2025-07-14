

- SceneKit
- SCNText
-  truncationMode 

Instance Property

# truncationMode

A constant that specifies how SceneKit truncates text that is too long to fit its container.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var truncationMode: String { get set }
```

## Discussion

When you define a layout rectangle for the text using its containerFrame property, SceneKit uses the truncationMode property to determine how to lay out text that does not fit in the layout rectangle. For possible values, see Truncation_modes in CATextLayer.

The default value of this property is none, specifying that SceneKit should not truncate the text. If the isWrapped property is true, SceneKit continues to automatically wrap each line of text beyond the height of the layout rectangle. Otherwise, SceneKit does not display text that would extend beyond the layout rectangle.

## See Also

### Managing Text Layout

var containerFrame: CGRect

A rectangle specifying the area in which SceneKit should lay out the text.

var isWrapped: Bool

A Boolean value that specifies whether SceneKit wraps long lines of text.

var alignmentMode: String

A constant that specifies how SceneKit horizontally aligns each line of text within its container.

var textSize: CGSize

The two-dimensional extent of the text after layout.

