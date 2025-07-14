

- AppKit
- NSTextLayoutManager
-  enumerateTextSegments(in:type:options:using:) 

Instance Method

# enumerateTextSegments(in:type:options:using:)

Enumerates text segments of a specific type and in the text range you provide.

macOS 12.0+

``` source
func enumerateTextSegments(
    in textRange: NSTextRange,
    type: NSTextLayoutManager.SegmentType,
    options: NSTextLayoutManager.SegmentOptions = [],
    using block: (NSTextRange?, CGRect, CGFloat, NSTextContainer) -> Bool
)
```

## Parameters 

`textRange`  

The range as an NSTextRange.

`type`  

One of the available NSTextLayoutManager.SegmentType values.

`options`  

One or more of the NSTextLayoutManager.SegmentOptions options.

`block`  

A closure you provide to determine if the enumeration finishes early.

## Discussion

A text segment is a logically and visually contiguous portion of the text content inside a line fragment that you specify with a single text range. The framework enumerates the segments visually from left to right. Returning `false` breaks out of the enumeration.

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

func replace(NSTextContentManager)

Replaces the current text content manager with a new one you provide.

func replaceContents(in: NSTextRange, with: NSAttributedString)

Replaces content at the location you specify with an attributed string you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement])

Replaces content at the location you specify with the text elements string you provide.

