

- AppKit
- NSView
-  showDefinition(for:at:) 

Instance Method

# showDefinition(for:at:)

Shows a window displaying the definition of the attributed string at the specified point.

macOS 10.6+

``` source
@MainActor
func showDefinition(
    for attrString: NSAttributedString?,
    at textBaselineOrigin: NSPoint
)
```

## Parameters 

`attrString`  

The attributed string for which to show the definition. If the view is an instance of NSTextView, the `attrString` can be `nil`, in which case the text view will automatically supply values suitable for displaying definitions for the specified range within its text content.

`textBaselineOrigin`  

Specifies the baseline origin of `attrString` in the view’s coordinate system.

## Discussion

Shows a window that displays the definition (or other subject depending on available dictionaries) of the specified attributed string.

This method can be used for implementing the same functionality as the `NSTextView` “Look Up in Dictionary” contextual menu on a custom view.

## See Also

### Displaying Definition Windows

func showDefinition(for: NSAttributedString?, range: NSRange, options: [NSView.DefinitionOptionKey : Any]?, baselineOriginProvider: ((NSRange) -> NSPoint)?)

Shows a window displaying the definition of the specified range of the attributed string.

struct DefinitionOptionKey

Keys to include in your definition.

struct DefinitionPresentationType

Presentation options for the window.

