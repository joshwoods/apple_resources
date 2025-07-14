

- UIKit
- UITextView
-  text 

Instance Property

# text

The text that the text view displays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var text: String! { get set }
```

## Discussion

In iOS 6 and later, assigning a new value to this property also replaces the value of the attributedText property with the same text, albeit without any inherent style attributes. Instead the text view styles the new string using the font, textColor, and other style-related properties of the class.

## See Also

### Specifying the text content

var attributedText: NSAttributedString!

The styled text that the text view displays.

