

- UIKit
- UITableViewRowAction
-  init(style:title:handler:) Deprecated

Initializer

# init(style:title:handler:)

Creates and returns a new table view row action object.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
convenience init(
    style: UITableViewRowAction.Style,
    title: String?,
    handler: @escaping (UITableViewRowAction, IndexPath) -> Void
)
```

## Parameters 

`style`  

The style characteristics to apply to the button. You use this value to apply default appearance characteristics to the button. These characteristics impart information about what the button does. For example, use this to indicate an action is destructive to the underlying data. For a list of possible style values, see UITableViewRowAction.Style.

`title`  

The string to display in the button. Specify a string localized for the user’s current language.

`handler`  

The block to execute when the user taps the button associated with this action. UIKit makes a copy of the block you provide. When the user selects the action represented by this object, UIKit executes your `handler` block on the app’s main thread. This parameter must not be `nil`. This block has no return value and takes the following parameters:

action  
The action object representing the action that the user selected.

indexPath  
The table row that the user acted on.

## Return Value

A new table row action object that you can return from your table view’s delegate method.

## Discussion

The style and handler block you specify can’t be changed later. You can change the title of the action button. You can also configure other appearance-related properties of the button using the properties of this class.

You can assign the same row action object to multiple rows of your table.

