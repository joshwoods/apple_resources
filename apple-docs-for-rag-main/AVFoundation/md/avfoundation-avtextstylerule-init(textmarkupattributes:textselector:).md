

- AVFoundation
- AVTextStyleRule
-  init(textMarkupAttributes:textSelector:) 

Initializer

# init(textMarkupAttributes:textSelector:)

Creates a text style rule object with the specified style attributes and text range information.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init?(
    textMarkupAttributes: [String : Any] = [:],
    textSelector: String?
)
```

## Parameters 

`textMarkupAttributes`  

A dictionary of style attributes. For a list of supported keys and values that you can include in this dictionary, see `CMTextMarkup.h`.

`textSelector`  

A string contains an identifier for the ranges of text to which the style attributes should be applied. Eligible identifiers are determined by the media format and its corresponding text content. For example, the string could contain the CSS selectors used by the corresponding text in Web Video Text Tracks (WebVTT) markup. Specify `nil` if you want the style attributes to apply to all text in the item.

## Return Value

A text style rule object initialized with the specified attributes and range information.

## See Also

### Creating and Initializing Style Rules

class func textStyleRules(fromPropertyList: Any) -> [AVTextStyleRule]?

Creates an array of text style rule objects from the specified property-list object.

convenience init?(textMarkupAttributes: [String : Any])

Creates a text style rule object with the specified style attributes.

