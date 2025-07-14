

- AppKit
- NSView
-  showDefinition(for:range:options:baselineOriginProvider:) 

Instance Method

# showDefinition(for:range:options:baselineOriginProvider:)

Shows a window displaying the definition of the specified range of the attributed string.

macOS 10.6+

``` source
@MainActor
func showDefinition(
    for attrString: NSAttributedString?,
    range targetRange: NSRange,
    options: [NSView.DefinitionOptionKey : Any]? = nil,
    baselineOriginProvider originProvider: ((NSRange) -> NSPoint)? = nil
)
```

## Parameters 

`attrString`  

The attributed string for which to show the definition. If the view is an instance of NSTextView, the `attrString` value can be `nil`, in which case the text view will automatically supply values suitable for displaying definitions for the specified range within its text content.

`targetRange`  

The range of the attributed string to define. You can pass a zero-length range and the appropriate range will be auto-detected around the range’s offset. That’s the recommended approach when there is no selection.

`options`  

An optional dictionary that specifies how the definition is displayed. See `NSDefinition Presentation Constants` for the key and it’s possible values.

`originProvider`  

The originProvider block object should return the baseline origin for the first character at the adjusted range.

If the view is an instance of NSTextView, the originProvider can be `NULL`, in which case the text view will automatically supply values suitable for displaying definitions for the specified range within its text content.

The block object takes a single argument:

adjustedRange  
The adjusted range.

The block object returns an `NSPoint` to be used as the baseline origin of the first character, in the view’s view coordinate system.

## Discussion

This method does not cause scrolling, so clients should perform any necessary scrolling before calling this method.

## See Also

### Displaying Definition Windows

func showDefinition(for: NSAttributedString?, at: NSPoint)

Shows a window displaying the definition of the attributed string at the specified point.

struct DefinitionOptionKey

Keys to include in your definition.

struct DefinitionPresentationType

Presentation options for the window.

