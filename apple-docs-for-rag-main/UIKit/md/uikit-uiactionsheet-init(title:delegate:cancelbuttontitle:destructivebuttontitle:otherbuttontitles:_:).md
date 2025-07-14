

- UIKit
- UIActionSheet
-  init(title:delegate:cancelButtonTitle:destructiveButtonTitle:otherButtonTitles:\_:) 

Initializer

# init(title:delegate:cancelButtonTitle:destructiveButtonTitle:otherButtonTitles:\_:)

Creates an action sheet with the specified values.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst

``` source
@MainActor @preconcurrency
convenience init(
    title: String?,
    delegate: (any UIActionSheetDelegate)?,
    cancelButtonTitle: String?,
    destructiveButtonTitle: String?,
    otherButtonTitles firstButtonTitle: String,
    _ moreButtonTitles: String...
)
```

## See Also

### Creating action sheets

init(title: String?, delegate: (any UIActionSheetDelegate)?, cancelButtonTitle: String?, destructiveButtonTitle: String?)

Initializes the action sheet using the specified starting parameters.

Deprecated

