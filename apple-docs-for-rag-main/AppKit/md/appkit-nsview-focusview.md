

- AppKit
- NSView
-  focusView 

Type Property

# focusView

The currently focused view object.

macOS

``` source
@MainActor
class var focusView: NSView? { get }
```

## Discussion

The value in this property is `nil` if there is no focused view.

