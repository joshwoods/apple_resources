

- TVMLKit
- TVTextElement
-  makeAttributedString(font:foregroundColor:textAlignment:) Deprecated

Instance Method

# makeAttributedString(font:foregroundColor:textAlignment:)

Convenience method for configuring an attributed string given the specified attributes.

tvOS 9.0–18.0Deprecated

``` source
func makeAttributedString(
    font: UIFont,
    foregroundColor: UIColor?,
    textAlignment alignment: NSTextAlignment
) -> NSAttributedString
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`font`  

The font used for the attributed string. This can be any available font on the device.

`foregroundColor`  

The foreground color for the element.

`alignment`  

The alignment for the text contained within the element.

## Return Value

An NSAttributedString object with the applied attributes.

## Discussion

Supply a font to this method to get the NSAttributedString representation of the text contained within an element. Use the `foregroundColor` and `alignment` parameters to override the value specified in the text element.

## See Also

### Creating Attributed Strings

func makeAttributedString(font: UIFont) -> NSAttributedString

Provides an attributed string for a given font.

Deprecated

