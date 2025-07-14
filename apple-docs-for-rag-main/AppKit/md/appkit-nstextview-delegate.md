

- AppKit
- NSTextView
-  delegate 

Instance Property

# delegate

The delegate for all text views sharing the receiver’s layout manager.

macOS

``` source
@MainActor
weak var delegate: (any NSTextViewDelegate)? { get set }
```

## See Also

### Managing the text view’s content

protocol NSTextViewDelegate

A set of optional methods that text view delegates can use to manage selection, set text attributes, work with the spell checker, and more.

