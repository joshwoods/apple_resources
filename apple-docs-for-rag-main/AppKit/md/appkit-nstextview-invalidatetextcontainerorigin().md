

- AppKit
- NSTextView
-  invalidateTextContainerOrigin() 

Instance Method

# invalidateTextContainerOrigin()

Invalidates the calculated origin of the text container.

macOS

``` source
@MainActor
func invalidateTextContainerOrigin()
```

## Discussion

This method is invoked automatically; you should never need to invoke it directly. Usually called because the text view has been resized or the contents of the text container have changed.

## See Also

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

var textLayoutManager: NSTextLayoutManager?

The manager that lays out text for the receiver’s text container.

var layoutManager: NSLayoutManager?

The layout manager that lays out text for the receiver’s text container.

var textContentStorage: NSTextContentStorage?

The receiver’s text storage object.

var textStorage: NSTextStorage?

The receiver’s text storage object.

