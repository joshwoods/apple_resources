

- UIKit
- NSTextLayoutManager
-  textContainer 

Instance Property

# textContainer

The text container object that provides geometric information for the layout destination.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var textContainer: NSTextContainer? { get set }
```

## See Also

### Accessing the text storage

var textContentManager: NSTextContentManager?

Returns the text content manager associated with this text layout manager.

var textSelectionNavigation: NSTextSelectionNavigation

Returns a text selection manager configured to have the text layout manager as its data source.

var textSelections: [NSTextSelection]

An array of text selections associated by the text layout manager.

var usageBoundsForTextContainer: CGRect

Returns the usage bounds for the text container.

func enumerateTextSegments(in: NSTextRange, type: NSTextLayoutManager.SegmentType, options: NSTextLayoutManager.SegmentOptions, using: (NSTextRange?, CGRect, CGFloat, NSTextContainer) -> Bool)

Enumerates text segments of a specific type and in the text range you provide.

func replace(NSTextContentManager)

Replaces the current text content manager with a new one you provide.

func replaceContents(in: NSTextRange, with: NSAttributedString)

Replaces content at the location you specify with an attributed string you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement])

Replaces content at the location you specify with the text elements string you provide.

