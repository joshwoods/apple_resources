

- AppKit
- NSTextView
-  usesInspectorBar 

Instance Property

# usesInspectorBar

A Boolean value that indicates whether this text view uses the inspector bar.

macOS 10.7+

``` source
@MainActor
var usesInspectorBar: Bool { get set }
```

## Discussion

The inspector bar displays text formatting controls, much like those in iWork applications, which can be used in place of the formatting controls in the ruler accessory view.

## See Also

### Using text formatting controls

var usesRuler: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager use a ruler.

var isRulerVisible: Bool

A Boolean value that controls whether the scroll view enclosing text views sharing the receiver’s layout manager displays the ruler.

