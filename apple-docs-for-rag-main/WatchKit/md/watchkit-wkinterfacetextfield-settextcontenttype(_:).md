

- WatchKit
- WKInterfaceTextField
-  setTextContentType(\_:) 

Instance Method

# setTextContentType(\_:)

Sets the text field’s semantic meaning.

watchOS 6.0+

``` source
func setTextContentType(_ textContentType: WKTextContentType?)
```

## Parameters 

`textContentType`  

The text field’s content type. Passing `nil` clears the content type. For a list of possible content types, see WKTextContentType.

## Discussion

The text field’s content type modifies how the text input controller and Apple Continuity Keyboard behave.

- The input controller provides suggestions for oneTimeCode content types, when available.

- The input controller displays a number pad for telephoneNumber, creditCardNumber, oneTimeCode, and postalCode content types.

- The input controller disables dictation for password and newPassword content types.

- The Apple Continuity Keyboard autofills data based on the content type. To share login credentials from your web page, set up an associated domain for your watchOS app.

## See Also

### Specifying the Content Type

struct WKTextContentType

Constants that specify a text field’s semantic meaning.

