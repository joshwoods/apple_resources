

- Finder Sync
- FIFinderSyncProtocol
-  requestBadgeIdentifier(for:) 

Instance Method

# requestBadgeIdentifier(for:)

Requests a badge for the given file or directory.

macOS 10.10+

``` source
optional func requestBadgeIdentifier(for url: URL)
```

## Parameters 

`url`  

The URL of a file or directory inside the extension’s monitored directories.

## Discussion

Override this method to receive notifications whenever a new item becomes visible in the Finder. Check the item’s state, and call setBadgeIdentifier(_:for:) to set an appropriate badge.

## See Also

### Related Documentation

func setBadgeIdentifier(String, for: URL)

Sets the badge for a file or directory.

### Managing Badges, Shortcut Menus, and Toolbar Buttons

func beginObservingDirectory(at: URL)

Tells the extension that the user is looking at a monitored directory or at one of its subdirectories.

func endObservingDirectory(at: URL)

Tells the extension that the user has stopped looking at a monitored directory or at one of its subdirectories.

func menu(for: FIMenuKind) -> NSMenu?

Requests a custom menu from the extension.

var toolbarItemImage: NSImage

The image for the extension’s toolbar button.

var toolbarItemName: String

The name of the extension’s toolbar button.

var toolbarItemToolTip: String

The tooltip text for the extension’s toolbar button.

