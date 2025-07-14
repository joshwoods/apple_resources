

- AppKit
- NSTextView
-  replaceTextContainer(\_:) 

Instance Method

# replaceTextContainer(\_:)

Replaces the text container for the group of text system objects containing the receiver, keeping the association between the receiver and its layout manager intact.

macOS

``` source
@MainActor
func replaceTextContainer(_ newContainer: NSTextContainer)
```

## Parameters 

`newContainer`  

The new text container. This method raises `NSInvalidArgumentException` if `aTextContainer` is `nil`.

## See Also

### Related Documentation

init(frame: NSRect, textContainer: NSTextContainer?)

Initializes a text view.

### Accessing text system objects

class var stronglyReferencesTextStorage: Bool

class func fieldEditor() -> Self

var textContainer: NSTextContainer?

The receiver’s text container.

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

