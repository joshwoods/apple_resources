

- AppKit
- NSMatrix
-  delegate 

Instance Property

# delegate

The delegate for messages from the field editor.

macOS

``` source
@MainActor
weak var delegate: (any NSMatrixDelegate)? { get set }
```

## See Also

### Related Documentation

func textShouldEndEditing(NSText) -> Bool

Requests permission to end editing.

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing text.

### Managing the Delegate

protocol NSMatrixDelegate

The `NSMatrixDelegate` protocol defines the optional methods implemented by delegates of `NSMatrix` objects.

