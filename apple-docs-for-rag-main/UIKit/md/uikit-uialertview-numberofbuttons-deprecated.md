

- UIKit
- UIAlertView
-  numberOfButtons Deprecated

Instance Property

# numberOfButtons

The number of buttons on the alert view.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var numberOfButtons: Int { get }
```

## See Also

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a button to the receiver with the given title.

Deprecated

func buttonTitle(at: Int) -> String?

Returns the title of the button at the given index.

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

