

- AVFoundation
- AVTextStyleRule
-  textSelector 

Instance Property

# textSelector

A string that identifies the text to which the attributes should apply.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var textSelector: String? { get }
```

## Discussion

The contents of the string are determined by the format of the legible media. For example, the string could contain the CSS selectors used by the corresponding text in Web Video Text Tracks (WebVTT) markup.

If the value of this property is `nil`, the text style attributes apply to all text in the media item.

## See Also

### Accessing the Style Attributes

var textMarkupAttributes: [String : Any]

A dictionary of text style attributes to apply to the text.

