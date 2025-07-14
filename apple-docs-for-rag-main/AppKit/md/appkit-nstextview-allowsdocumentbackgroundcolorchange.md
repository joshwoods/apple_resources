

- AppKit
- NSTextView
-  allowsDocumentBackgroundColorChange 

Instance Property

# allowsDocumentBackgroundColorChange

A Boolean value that indicates whether the receiver allows its background color to change.

macOS

``` source
@MainActor
var allowsDocumentBackgroundColorChange: Bool { get set }
```

## Discussion

true if the receiver allows the background color to change, otherwise false.

## See Also

### Setting graphics attributes

var backgroundColor: NSColor

The receiver’s background color.

var drawsBackground: Bool

A Boolean value that indicates whether the receiver draws its background.

func changeDocumentBackgroundColor(Any?)

An action method used to set the background color.

