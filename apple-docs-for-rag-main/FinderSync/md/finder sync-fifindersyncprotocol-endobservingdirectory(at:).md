

- Finder Sync
- FIFinderSyncProtocol
-  endObservingDirectory(at:) 

Instance Method

# endObservingDirectory(at:)

Tells the extension that the user has stopped looking at a monitored directory or at one of its subdirectories.

macOS 10.10+

``` source
optional func endObservingDirectory(at url: URL)
```

## Parameters 

`url`  

The URL of the directory.

## Discussion

Override this method to receive notifications when the user is no longer looking at the contents of the given URL. As with beginObservingDirectory(at:), the Open and Save dialogs are tracked separately from the Finder.

## See Also

### Managing Badges, Shortcut Menus, and Toolbar Buttons

func beginObservingDirectory(at: URL)

Tells the extension that the user is looking at a monitored directory or at one of its subdirectories.

func menu(for: FIMenuKind) -> NSMenu?

Requests a custom menu from the extension.

func requestBadgeIdentifier(for: URL)

Requests a badge for the given file or directory.

var toolbarItemImage: NSImage

The image for the extension’s toolbar button.

var toolbarItemName: String

The name of the extension’s toolbar button.

var toolbarItemToolTip: String

The tooltip text for the extension’s toolbar button.

