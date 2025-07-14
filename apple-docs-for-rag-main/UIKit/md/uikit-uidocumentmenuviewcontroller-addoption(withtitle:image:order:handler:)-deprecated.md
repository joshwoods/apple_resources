

- UIKit
- UIDocumentMenuViewController
-  addOption(withTitle:image:order:handler:) Deprecated

Instance Method

# addOption(withTitle:image:order:handler:)

Adds a custom menu item to the list of document pickers.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func addOption(
    withTitle title: String,
    image: UIImage?,
    order: UIDocumentMenuOrder,
    handler: @escaping () -> Void
)
```

## Parameters 

`title`  

The custom menu item’s title.

`image`  

The custom menu item’s image.

`order`  

The position of this menu item. See UIDocumentMenuOrder for possible values.

`handler`  

A block that is called when the user selects this custom menu item.

## See Also

### Configuring a document menu

enum UIDocumentMenuOrder

The insertion point for custom menu items.

Deprecated

