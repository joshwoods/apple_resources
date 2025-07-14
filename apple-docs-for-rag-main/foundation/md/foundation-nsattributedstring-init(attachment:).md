

- Foundation
- NSAttributedString
-  init(attachment:) 

Initializer

# init(attachment:)

Creates an attributed string with an attachment.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(attachment: NSTextAttachment)
```

## Parameters 

`attachment`  

The attrachment to place in the string.

## Return Value

An attributed string containing the attachment.

## Discussion

This is a convenience method for creating an attributed string containing an attachment using character as the base character.

## See Also

### Creating a string with an attachment

convenience init(attachment: NSTextAttachment, attributes: [NSAttributedString.Key : Any])

Creates an attributed string with an attachment and applies the specified attributes to it.

convenience init(adaptiveImageGlyph: NSAdaptiveImageGlyph, attributes: [NSAttributedString.Key : Any])

Creates an attributed string with an adaptive image glyph and applies the specified attributes to it.

