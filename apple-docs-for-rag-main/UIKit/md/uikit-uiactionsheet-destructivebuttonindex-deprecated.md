

- UIKit
- UIActionSheet
-  destructiveButtonIndex Deprecated

Instance Property

# destructiveButtonIndex

The index number of the destructive button.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var destructiveButtonIndex: Int { get set }
```

## Discussion

Button indices start at `0`. The default value of this property is normally `-1`, which indicates that no destructive button has been set. However, a destructive button may be created and set automatically by the init(title:delegate:cancelButtonTitle:destructiveButtonTitle:) method. If you use that method to create a destructive button, you should not change the value of this property.

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

var firstOtherButtonIndex: Int

The index of the first custom button.

Deprecated

