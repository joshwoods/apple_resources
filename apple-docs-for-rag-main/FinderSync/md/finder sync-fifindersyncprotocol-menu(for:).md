

- Finder Sync
- FIFinderSyncProtocol
-  menu(for:) 

Instance Method

# menu(for:)

Requests a custom menu from the extension.

macOS 10.10+

``` source
optional func menu(for menu: FIMenuKind) -> NSMenu?
```

## Parameters 

`menu`  

The type of menu being displayed. For a list of possible values, see FIMenuKind.

## Return Value

A custom menu.

## Discussion

Override this method to provide custom menus in the Finder. You can customize this menu based both on the menu’s kind and on the selected and targeted items (if any). You can get the selected and targeted items from the extension’s FIFinderSyncController.

If `kind` is `FIMenuKindToolbarItemMenu`, the system always calls this method even if the target and selection are not related to the extension.

The extension’s principal object provides a method for each menu item’s assigned action.

## See Also

### Related Documentation

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

func selectedItemURLs() -> [URL]?

Returns an array of selected items.

### Managing Badges, Shortcut Menus, and Toolbar Buttons

func beginObservingDirectory(at: URL)

Tells the extension that the user is looking at a monitored directory or at one of its subdirectories.

func endObservingDirectory(at: URL)

Tells the extension that the user has stopped looking at a monitored directory or at one of its subdirectories.

func requestBadgeIdentifier(for: URL)

Requests a badge for the given file or directory.

var toolbarItemImage: NSImage

The image for the extension’s toolbar button.

var toolbarItemName: String

The name of the extension’s toolbar button.

var toolbarItemToolTip: String

The tooltip text for the extension’s toolbar button.

