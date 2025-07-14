

- UIKit
- UITextItem
- UITextItem.MenuConfiguration
-  init(preview:menu:) 

Initializer

# init(preview:menu:)

Creates a text item menu configuration with the specified menu and preview.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(
    preview: UITextItem.MenuConfiguration.Preview? = .default,
    menu: UIMenu
)
```

## Parameters 

`preview`  

The preview to display alongside the menu.

`menu`  

The menu to present when the user interacts with the text item.

## See Also

### Creating a menu configuration

enum Preview

Constants that indicate what type of preview to display alongside the text item’s menu.

