

- AppKit
- NSTextView
-  usesRuler 

Instance Property

# usesRuler

A Boolean value that controls whether the text views sharing the receiver’s layout manager use a ruler.

macOS

``` source
@MainActor
var usesRuler: Bool { get set }
```

## Discussion

true to cause text views sharing the receiver’s layout manager to respond to NSRulerView client messages and to paragraph-related menu actions, and update the ruler (when visible) as the selection changes with its paragraph and tab attributes, otherwise false.

## See Also

### Related Documentation

var rangeForUserParagraphAttributeChange: NSRange

The range of characters affected by an action method that changes paragraph (not character) attributes.

### Using text formatting controls

var isRulerVisible: Bool

A Boolean value that controls whether the scroll view enclosing text views sharing the receiver’s layout manager displays the ruler.

var usesInspectorBar: Bool

A Boolean value that indicates whether this text view uses the inspector bar.

