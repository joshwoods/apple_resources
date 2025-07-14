

- UIKit
- UIResponder
-  textInputContextIdentifier 

Instance Property

# textInputContextIdentifier

An identifier signifying that the responder should preserve its text input mode information.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var textInputContextIdentifier: String? { get }
```

## Discussion

If you redefine this property and return a string value, UIKit tracks the current text input mode for the responder. While in tracking mode, any programmatic changes you make to the text input mode are remembered and restored whenever the responder becomes active.

## See Also

### Managing the text input mode

var textInputMode: UITextInputMode?

The text input mode for this responder object.

class func clearTextInputContextIdentifier(String)

Clears text input mode information from the app’s user defaults.

var inputAssistantItem: UITextInputAssistantItem

The input assistant to use when configuring the keyboard’s shortcuts bar.

