

- AppKit
- NSTextView
-  textContainerOrigin 

Instance Property

# textContainerOrigin

The origin of the receiver’s text container.

macOS

``` source
@MainActor
var textContainerOrigin: NSPoint { get }
```

## Discussion

Calculated from the receiver’s bounds rectangle, container inset, and the container’s used rect.

## See Also

### Related Documentation

func usedRect(for: NSTextContainer) -> NSRect

Returns the bounding rectangle for the glyphs in the specified text container.

### Accessing text system objects

class var stronglyReferencesTextStorage: Bool

class func fieldEditor() -> Self

var textContainer: NSTextContainer?

The receiver’s text container.

func replaceTextContainer(NSTextContainer)

Replaces the text container for the group of text system objects containing the receiver, keeping the association between the receiver and its layout manager intact.

var textContainerInset: NSSize

The empty space the receiver leaves around its associated text container.

func invalidateTextContainerOrigin()

Invalidates the calculated origin of the text container.

var textLayoutManager: NSTextLayoutManager?

The manager that lays out text for the receiver’s text container.

var layoutManager: NSLayoutManager?

The layout manager that lays out text for the receiver’s text container.

var textContentStorage: NSTextContentStorage?

The receiver’s text storage object.

var textStorage: NSTextStorage?

The receiver’s text storage object.

