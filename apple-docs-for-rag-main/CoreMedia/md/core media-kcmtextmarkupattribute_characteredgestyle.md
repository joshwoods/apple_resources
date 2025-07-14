

- Core Media
-  kCMTextMarkupAttribute_CharacterEdgeStyle 

Global Variable

# kCMTextMarkupAttribute_CharacterEdgeStyle

A style for character edges.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_CharacterEdgeStyle: CFString
```

## Discussion

This attribute’s value must be one of the constants listed below that control the shape of the edges of drawn characters. The default value is kCMTextMarkupCharacterEdgeStyle_None.

## Topics

### Edge Styles

let kCMTextMarkupCharacterEdgeStyle_None: CFString

No edge style.

let kCMTextMarkupCharacterEdgeStyle_Raised: CFString

A raised edge style.

let kCMTextMarkupCharacterEdgeStyle_Depressed: CFString

A depressed edge style.

let kCMTextMarkupCharacterEdgeStyle_Uniform: CFString

A uniform border style.

let kCMTextMarkupCharacterEdgeStyle_DropShadow: CFString

A drop shadow style.

## See Also

### Styles

let kCMTextMarkupAttribute_BoldStyle: CFString

A bold font style.

let kCMTextMarkupAttribute_ItalicStyle: CFString

An italic font style.

let kCMTextMarkupAttribute_UnderlineStyle: CFString

An underline font style.

