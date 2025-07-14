

- AVFoundation
- AVTextStyleRule
-  textMarkupAttributes 

Instance Property

# textMarkupAttributes

A dictionary of text style attributes to apply to the text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var textMarkupAttributes: [String : Any] { get }
```

## Discussion

The supported keys for this dictionary are defined in `CMTextMarkup.h`.

## See Also

### Accessing the Style Attributes

var textSelector: String?

A string that identifies the text to which the attributes should apply.

