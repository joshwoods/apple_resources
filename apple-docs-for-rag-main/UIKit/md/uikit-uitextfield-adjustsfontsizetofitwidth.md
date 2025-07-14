

- UIKit
- UITextField
-  adjustsFontSizeToFitWidth 

Instance Property

# adjustsFontSizeToFitWidth

A Boolean value that indicates whether to reduce the font size to fit the text string into the text field’s bounding rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var adjustsFontSizeToFitWidth: Bool { get set }
```

## Discussion

Normally, the text field’s content is drawn with the font you specify in the font property. If this property is set to true, however, and the contents in the text property exceed the text field’s bounding rectangle, the receiver starts reducing the font size until the string fits or the minimum font size is reached. The text is shrunk along the baseline.

The default value for this property is false. If you change it to true, you should also set an appropriate minimum font size by modifying the minimumFontSize property.

## See Also

### Sizing the text field’s text

var minimumFontSize: CGFloat

The size of the smallest permissible font when drawing the text field’s text.

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

