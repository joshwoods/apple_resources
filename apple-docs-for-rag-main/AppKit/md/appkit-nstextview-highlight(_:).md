

- AppKit
- NSTextView
-  highlight(\_:) 

Instance Method

# highlight(\_:)

An action for toggling `NSTextHighlightStyleAttributeName` in the receiver’s selected range. The sender should be a menu item with a `representedObject` of type (`NSTextHighlightColorScheme`).

macOS 15.0+

``` source
@IBAction @MainActor
func highlight(_ sender: Any?)
```

