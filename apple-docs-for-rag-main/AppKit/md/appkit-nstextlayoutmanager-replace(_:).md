

- AppKit
- NSTextLayoutManager
-  replace(\_:) 

Instance Method

# replace(\_:)

Replaces the current text content manager with a new one you provide.

macOS 12.0+

``` source
func replace(_ textContentManager: NSTextContentManager)
```

## Parameters 

`textContentManager`  

The new text context manager.

## Discussion

Use this method to replace the current NSTextContentManager with a new one, leaving all related objects intact. This method makes sure the NSTextLayoutManager doesn’t get deallocated while migrating to the new manager.

## See Also

### Accessing the text storage

var textContentManager: NSTextContentManager?

Returns the text content manager associated with this text layout manager.

var textContainer: NSTextContainer?

The text container object that provides geometric information for the layout destination.

var textSelectionNavigation: NSTextSelectionNavigation

Returns a text selection manager configured to have the text layout manager as its data source.

var textSelections: [NSTextSelection]

An array of text selections associated by the text layout manager.

var usageBoundsForTextContainer: CGRect

Returns the usage bounds for the text container.

func enumerateTextSegments(in: NSTextRange, type: NSTextLayoutManager.SegmentType, options: NSTextLayoutManager.SegmentOptions, using: (NSTextRange?, CGRect, CGFloat, NSTextContainer) -> Bool)

Enumerates text segments of a specific type and in the text range you provide.

func replaceContents(in: NSTextRange, with: NSAttributedString)

Replaces content at the location you specify with an attributed string you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement])

Replaces content at the location you specify with the text elements string you provide.

