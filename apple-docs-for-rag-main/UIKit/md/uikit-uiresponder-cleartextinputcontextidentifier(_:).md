

- UIKit
- UIResponder
-  clearTextInputContextIdentifier(\_:) 

Type Method

# clearTextInputContextIdentifier(\_:)

Clears text input mode information from the app’s user defaults.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func clearTextInputContextIdentifier(_ identifier: String)
```

## Parameters 

`identifier`  

An identifier assigned to the textInputContextIdentifier property of one of your responders.

## Discussion

Calling this method removes any text input mode information associated with the specified identifier from the app’s user defaults. Removing this information causes the responder to use the default text input mode again.

## See Also

### Managing the text input mode

var textInputMode: UITextInputMode?

The text input mode for this responder object.

var textInputContextIdentifier: String?

An identifier signifying that the responder should preserve its text input mode information.

var inputAssistantItem: UITextInputAssistantItem

The input assistant to use when configuring the keyboard’s shortcuts bar.

