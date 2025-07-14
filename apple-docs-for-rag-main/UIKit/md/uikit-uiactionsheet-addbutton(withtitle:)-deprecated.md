

- UIKit
- UIActionSheet
-  addButton(withTitle:) Deprecated

Instance Method

# addButton(withTitle:)

Adds a custom button to the action sheet.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func addButton(withTitle title: String?) -> Int
```

## Parameters 

`title`  

The title of the new button.

## Return Value

The index of the new button. Button indices start at `0` and increase in the order they are added.

## See Also

### Related Documentation

class UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

Deprecated

### Configuring buttons

var numberOfButtons: Int

The number of buttons on the action sheet.

Deprecated

func buttonTitle(at: Int) -> String?

Returns the title of the button at the specified index.

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

