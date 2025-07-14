

- UIKit
- UIAlertView
-  firstOtherButtonIndex Deprecated

Instance Property

# firstOtherButtonIndex

The index of the first other button.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var firstOtherButtonIndex: Int { get }
```

## Discussion

The button indices start at `0`. If `-1`, then the index is not set. This property is ignored if there are no other buttons. The default value is `-1`.

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

func textField(at: Int) -> UITextField?

Returns the text field at the given index

Deprecated

var cancelButtonIndex: Int

The index number of the cancel button.

Deprecated

