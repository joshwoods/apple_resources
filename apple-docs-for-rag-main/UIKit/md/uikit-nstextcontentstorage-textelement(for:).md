

- UIKit
- NSTextContentStorage
-  textElement(for:) 

Instance Method

# textElement(for:)

Returns the text element corresponding to object’s attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func textElement(for attributedString: NSAttributedString) -> NSTextElement?
```

## Parameters 

`attributedString`  

The attributed string to map into an NSTextElement.

## Return Value

An NSTextElement, or `nil`.

## Discussion

Returns `nil` when `attributedString` contains attributes not mappable to NSTextElement.

## See Also

### Managing text elements

func attributedString(for: NSTextElement) -> NSAttributedString?

Returns a new attributed string for the text element.

