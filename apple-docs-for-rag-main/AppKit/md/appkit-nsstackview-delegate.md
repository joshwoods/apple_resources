

- AppKit
- NSStackView
-  delegate 

Instance Property

# delegate

The delegate object for the stack view.

macOS 10.9+

``` source
@MainActor
weak var delegate: (any NSStackViewDelegate)? { get set }
```

## Discussion

The system calls a delegate method when resizing has caused a view to be detached from or reattached to the stack view. For more information, see NSStackViewDelegate.

## See Also

### Responding to Stack-Related Changes

protocol NSStackViewDelegate

A set of methods you use to respond to a stack view detaching and reattaching views.

