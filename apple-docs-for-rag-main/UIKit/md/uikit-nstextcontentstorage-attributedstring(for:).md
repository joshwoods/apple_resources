

- UIKit
- NSTextContentStorage
-  attributedString(for:) 

Instance Method

# attributedString(for:)

Returns a new attributed string for the text element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func attributedString(for textElement: NSTextElement) -> NSAttributedString?
```

## Parameters 

`textElement`  

The NSTextElement to map into an attributed string.

## Return Value

An NSAttributedString, or `nil`.

## Discussion

Returns `nil` if the method can’t map `textElement` to an NSAttributedString.

## See Also

### Managing text elements

func textElement(for: NSAttributedString) -> NSTextElement?

Returns the text element corresponding to object’s attributed string.

