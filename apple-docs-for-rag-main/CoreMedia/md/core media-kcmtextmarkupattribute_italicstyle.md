

- Core Media
-  kCMTextMarkupAttribute_ItalicStyle 

Global Variable

# kCMTextMarkupAttribute_ItalicStyle

An italic font style.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_ItalicStyle: CFString
```

## Discussion

This attribute’s value must be a `CFBoolean`. The default is `kCFBooleanFalse`. If this attribute is `kCFBooleanTrue`, the system renders the text with an italic style in addition to other styles you use.

## See Also

### Styles

let kCMTextMarkupAttribute_BoldStyle: CFString

A bold font style.

let kCMTextMarkupAttribute_UnderlineStyle: CFString

An underline font style.

let kCMTextMarkupAttribute_CharacterEdgeStyle: CFString

A style for character edges.

