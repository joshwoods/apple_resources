

- UIKit
- UIActionSheet
-  firstOtherButtonIndex Deprecated

Instance Property

# firstOtherButtonIndex

The index of the first custom button.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var firstOtherButtonIndex: Int { get }
```

## Discussion

Button indices start at `0`. The default value of this property is `-1`, which indicates that there are no other custom buttons.

## See Also

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a custom button to the action sheet.

Deprecated

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

