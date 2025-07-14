

- AppKit
- NSTextView
-  textContainer 

Instance Property

# textContainer

The receiver’s text container.

macOS

``` source
@MainActor
unowned(unsafe) var textContainer: NSTextContainer? { get set }
```

## Discussion

The receiver uses the layout manager and text storage of `aTextContainer`.

## See Also

### Accessing text system objects

class var stronglyReferencesTextStorage: Bool

class func fieldEditor() -> Self

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

var layoutManager: NSLayoutManager?

The layout manager that lays out text for the receiver’s text container.

var textContentStorage: NSTextContentStorage?

The receiver’s text storage object.

var textStorage: NSTextStorage?

The receiver’s text storage object.

