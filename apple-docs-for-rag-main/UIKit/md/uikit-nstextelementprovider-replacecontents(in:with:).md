

- UIKit
- NSTextElementProvider
-  replaceContents(in:with:) 

Instance Method

# replaceContents(in:with:)

Replaces the characters specified by range with the text elements you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func replaceContents(
    in range: NSTextRange,
    with textElements: [NSTextElement]?
)
```

**Required**

## Parameters 

`range`  

An NSTextRange.

`textElements`  

The elements to replace that characters at `range`.

## Discussion

If the edges of `range` aren’t at existing element range boundaries, the method either splits the element if it allows the operation (for example, NSTextParagraph), or the adjusts the replacement range.

Note

This method is for use by NSTextLayoutManager.

## See Also

### Accessing and updating the text

func enumerateTextElements(from: (any NSTextLocation)?, options: NSTextContentManager.EnumerationOptions, using: (NSTextElement) -> Bool) -> (any NSTextLocation)?

Enumerates text elements starting at the text location you provide.

**Required**

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location from location with offset you provide.

