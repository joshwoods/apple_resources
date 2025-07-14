

- UIKit
- UIActionSheet
-  cancelButtonIndex Deprecated

Instance Property

# cancelButtonIndex

The index number of the cancel button.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var cancelButtonIndex: Int { get set }
```

## Discussion

Button indices start at `0`. The default value of this property is normally `-1`, which indicates that no cancel button has been set. However, a cancel button may be created and set automatically by the init(title:delegate:cancelButtonTitle:destructiveButtonTitle:) method. If you use that method to create a cancel button, you should not change the value of this property.

When presenting an action sheet on an iPad, there are times when you should not include a cancel button. For more information on when you should include a cancel button, see the class overview or iOS Human Interface Guidelines.

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

var destructiveButtonIndex: Int

The index number of the destructive button.

Deprecated

var firstOtherButtonIndex: Int

The index of the first custom button.

Deprecated

