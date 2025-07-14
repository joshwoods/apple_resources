

- AppKit
- NSTextView
-  layoutManager 

Instance Property

# layoutManager

The layout manager that lays out text for the receiver’s text container.

macOS

``` source
@MainActor
unowned(unsafe) var layoutManager: NSLayoutManager? { get }
```

## See Also

### Related Documentation

var layoutManager: NSLayoutManager?

The text container’s layout manager.

func replaceLayoutManager(NSLayoutManager)

Replaces the layout manager for the group of text system objects that contains the text container.

### Accessing text system objects

class var stronglyReferencesTextStorage: Bool

class func fieldEditor() -> Self

var textContainer: NSTextContainer?

The receiver’s text container.

func replaceTextContainer(NSTextContainer)

Replaces the text container for the group of text system objects containing the receiver, keeping the association between the receiver and its layout manager intact.

var textContainerInset: NSSize

The empty space the receiver leaves around its associated text container.

var textContainerOrigin: NSPoint

The origin of the receiver’s text container.

func invalidateTextContainerOrigin()

Invalidates the calculated origin of the text container.

var textLayoutManager: NSTextLayoutManager?

The manager that lays out text for the receiver’s text container.

var textContentStorage: NSTextContentStorage?

The receiver’s text storage object.

var textStorage: NSTextStorage?

The receiver’s text storage object.

