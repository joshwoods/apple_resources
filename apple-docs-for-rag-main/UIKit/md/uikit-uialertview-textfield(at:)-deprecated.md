

- UIKit
- UIAlertView
-  textField(at:) Deprecated

Instance Method

# textField(at:)

Returns the text field at the given index

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func textField(at textFieldIndex: Int) -> UITextField?
```

## Parameters 

`textFieldIndex`  

The index of the text field. The text field indices start at `0`.

## Return Value

The text field specified by index `textFieldIndex`.

## Discussion

The number of text fields present in an alert is dependent on the style of the alert.

| Alert Style | Text Fields |
|----|----|
| UIAlertViewStyle.default | No user-editable text fields. |
| UIAlertViewStyle.secureTextInput | A single text field at index `0`. |
| UIAlertViewStyle.plainTextInput | A single text field at index `0`. |
| UIAlertViewStyle.loginAndPasswordInput | The login field is at index `0`. The password field is at index `1`. |

If your application attempts to retrieve a text field with an index that is out of bounds, the alert raises an rangeException.

## See Also

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a button to the receiver with the given title.

Deprecated

var numberOfButtons: Int

The number of buttons on the alert view.

Deprecated

func buttonTitle(at: Int) -> String?

Returns the title of the button at the given index.

Deprecated

var cancelButtonIndex: Int

The index number of the cancel button.

Deprecated

var firstOtherButtonIndex: Int

The index of the first other button.

Deprecated

