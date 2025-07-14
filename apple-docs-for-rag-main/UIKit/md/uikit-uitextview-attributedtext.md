

- UIKit
- UITextView
-  attributedText 

Instance Property

# attributedText

The styled text that the text view displays.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@NSCopying @MainActor
var attributedText: NSAttributedString! { get set }
```

## Discussion

Assigning a new value to this property also replaces the value of the text property with the same string data, albeit without any formatting information. In addition, the font, textColor, and textAlignment properties are updated to reflect the typing attributes of the text view.

## See Also

### Specifying the text content

var text: String!

The text that the text view displays.

