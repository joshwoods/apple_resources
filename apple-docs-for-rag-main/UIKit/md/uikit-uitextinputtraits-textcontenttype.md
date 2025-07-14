

- UIKit
- UITextInputTraits
-  textContentType 

Instance Property

# textContentType

The semantic meaning for a text input area.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
optional var textContentType: UITextContentType! { get set }
```

## Discussion

Use this property to give the keyboard and the system information about the expected semantic meaning for the content that users enter. For example, you might specify emailAddress for a text field that users fill in to receive an email confirmation. When you provide this information about the content you expect users to enter in a text input area, the system can in some cases automatically select an appropriate keyboard and improve keyboard corrections and proactive integration with other text input opportunities.

Because the expected semantic meaning for each text input area should be identified as specifically as possible, you can’t combine multiple values for one textContentType property. For possible values you can use, see UITextContentType; by default, the value of this property is `nil`.

## See Also

### Configuring the keyboard appearance

var keyboardType: UIKeyboardType

The keyboard type for the text object.

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

var keyboardAppearance: UIKeyboardAppearance

The appearance style of the keyboard for the text object.

enum UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

var returnKeyType: UIReturnKeyType

The visible title of the Return key.

enum UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

struct UITextContentType

Constants that identify the semantic meaning for a text-entry area.

