

- AppKit
- NSTextView
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean value that indicates whether the receiver draws its background.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

true to cause the receiver to fill its background with the background color, false otherwise.

## See Also

### Setting graphics attributes

var backgroundColor: NSColor

The receiver’s background color.

var allowsDocumentBackgroundColorChange: Bool

A Boolean value that indicates whether the receiver allows its background color to change.

func changeDocumentBackgroundColor(Any?)

An action method used to set the background color.

