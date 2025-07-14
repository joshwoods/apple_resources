

- UIKit
- UIAlertView
-  buttonTitle(at:) Deprecated

Instance Method

# buttonTitle(at:)

Returns the title of the button at the given index.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func buttonTitle(at buttonIndex: Int) -> String?
```

## Parameters 

`buttonIndex`  

The index of the button. The button indices start at `0`.

## Return Value

The title of the button specified by index `buttonIndex`.

## See Also

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a button to the receiver with the given title.

Deprecated

var numberOfButtons: Int

The number of buttons on the alert view.

Deprecated

func textField(at: Int) -> UITextField?

Returns the text field at the given index

Deprecated

var cancelButtonIndex: Int

The index number of the cancel button.

Deprecated

var firstOtherButtonIndex: Int

The index of the first other button.

Deprecated

