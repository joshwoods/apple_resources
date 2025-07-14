

- SceneKit
- SCNText
-  isWrapped 

Instance Property

# isWrapped

A Boolean value that specifies whether SceneKit wraps long lines of text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isWrapped: Bool { get set }
```

## Discussion

When you define a layout rectangle for the text using its containerFrame property, SceneKit uses the isWrapped property to determine whether each line of text that is wider than the layout rectangle automatically wraps onto the next line.

The default value of this property is false, specifying that long lines of text do not wrap. (If you specify a container frame, long lines of text extend beyond its width.)

## See Also

### Managing Text Layout

var containerFrame: CGRect

A rectangle specifying the area in which SceneKit should lay out the text.

var alignmentMode: String

A constant that specifies how SceneKit horizontally aligns each line of text within its container.

var truncationMode: String

A constant that specifies how SceneKit truncates text that is too long to fit its container.

var textSize: CGSize

The two-dimensional extent of the text after layout.

