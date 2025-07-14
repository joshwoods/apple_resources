

- AppKit
- NSTextViewportLayoutController
-  delegate 

Instance Property

# delegate

The delegate for the text layout manager object.

macOS 12.0+

``` source
weak var delegate: (any NSTextViewportLayoutControllerDelegate)? { get set }
```

## See Also

### Responding to changes in viewport layout

protocol NSTextViewportLayoutControllerDelegate

Optional methods that delegates implement to respond to viewport layout changes.

