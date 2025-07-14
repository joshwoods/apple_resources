

- UIKit
- UIActionSheet
-  buttonTitle(at:) Deprecated

Instance Method

# buttonTitle(at:)

Returns the title of the button at the specified index.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

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

### Related Documentation

func show(in: UIView)

Displays an action sheet that originates from the specified view.

Deprecated

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a custom button to the action sheet.

Deprecated

var numberOfButtons: Int

The number of buttons on the action sheet.

Deprecated

var cancelButtonIndex: Int

The index number of the cancel button.

Deprecated

var destructiveButtonIndex: Int

The index number of the destructive button.

Deprecated

var firstOtherButtonIndex: Int

The index of the first custom button.

Deprecated

