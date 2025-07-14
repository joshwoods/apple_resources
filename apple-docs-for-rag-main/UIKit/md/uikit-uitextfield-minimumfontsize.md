

- UIKit
- UITextField
-  minimumFontSize 

Instance Property

# minimumFontSize

The size of the smallest permissible font when drawing the text field’s text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var minimumFontSize: CGFloat { get set }
```

## Discussion

When drawing text that might not fit within the bounding rectangle of the text field, you can use this property to prevent the receiver from reducing the font size to the point where it is no longer legible.

The default value for this property is 0.0. If you enable font adjustment for the text field, you should always increase this value.

If you are using styled text in iOS 6 or later, assigning a new value to this property causes the minimum font size to be applied to the entirety of the string in the attributedText property. If you want to apply different minimum font sizes to different parts of your string, create a new attributed string with the desired style information and associate it with the text field.

## See Also

### Sizing the text field’s text

var adjustsFontSizeToFitWidth: Bool

A Boolean value that indicates whether to reduce the font size to fit the text string into the text field’s bounding rectangle.

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

