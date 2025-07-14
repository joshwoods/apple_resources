

- UIKit
- UIAlertView
-  addButton(withTitle:) Deprecated

Instance Method

# addButton(withTitle:)

Adds a button to the receiver with the given title.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func addButton(withTitle title: String?) -> Int
```

## Parameters 

`title`  

The title of the new button.

## Return Value

The index of the new button. Button indices start at `0` and increase in the order they are added.

## Discussion

Adding too many buttons can cause the alert view to scroll. For guidelines on the best ways to use an alert in an app, see Temporary Views.

## See Also

### Related Documentation

var message: String?

Descriptive text that provides more details than the title.

Deprecated

### Configuring buttons

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

var firstOtherButtonIndex: Int

The index of the first other button.

Deprecated

