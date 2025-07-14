

- TVMLKit
- TVTextElement
-  makeAttributedString(font:) Deprecated

Instance Method

# makeAttributedString(font:)

Provides an attributed string for a given font.

tvOS 9.0–18.0Deprecated

``` source
func makeAttributedString(font: UIFont) -> NSAttributedString
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`font`  

The font used for the attributed string. This can be any available font on the device.

## Return Value

An NSAttributedString object with the supplied font.

## Discussion

Supply a font to this method to get the NSAttributedString representation of the text contained within an element.

## See Also

### Creating Attributed Strings

func makeAttributedString(font: UIFont, foregroundColor: UIColor?, textAlignment: NSTextAlignment) -> NSAttributedString

Convenience method for configuring an attributed string given the specified attributes.

Deprecated

