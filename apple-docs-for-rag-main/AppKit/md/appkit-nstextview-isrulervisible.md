

- AppKit
- NSTextView
-  isRulerVisible 

Instance Property

# isRulerVisible

A Boolean value that controls whether the scroll view enclosing text views sharing the receiver’s layout manager displays the ruler.

macOS

``` source
@MainActor
var isRulerVisible: Bool { get set }
```

## Discussion

true to show the ruler, false to hide the ruler. By default, the ruler is hidden.

## See Also

### Related Documentation

func toggleRuler(Any?)

This action method shows or hides the ruler, if the receiver is enclosed in a scroll view.

### Using text formatting controls

var usesRuler: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager use a ruler.

var usesInspectorBar: Bool

A Boolean value that indicates whether this text view uses the inspector bar.

