

- Foundation
- NSAttributedString
-  init(adaptiveImageGlyph:attributes:) 

Initializer

# init(adaptiveImageGlyph:attributes:)

Creates an attributed string with an adaptive image glyph and applies the specified attributes to it.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    adaptiveImageGlyph: NSAdaptiveImageGlyph,
    attributes: [NSAttributedString.Key : Any] = [:]
)
```

## Parameters 

`adaptiveImageGlyph`  

The adaptive image glyph to place in the string. Typically, you get this type from the text input system.

`attributes`  

The attributes to apply to the adaptive image glyph. Specify an empty dictionary to create the string without any extra attributes.

## Return Value

An attributed string containing the adaptive image glyph.

## See Also

### Creating a string with an attachment

init(attachment: NSTextAttachment)

Creates an attributed string with an attachment.

convenience init(attachment: NSTextAttachment, attributes: [NSAttributedString.Key : Any])

Creates an attributed string with an attachment and applies the specified attributes to it.

