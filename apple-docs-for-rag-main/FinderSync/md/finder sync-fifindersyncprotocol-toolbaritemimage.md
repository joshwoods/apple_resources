

- Finder Sync
- FIFinderSyncProtocol
-  toolbarItemImage 

Instance Property

# toolbarItemImage

The image for the extension’s toolbar button.

macOS 10.10+

``` source
@NSCopying
optional var toolbarItemImage: NSImage { get }
```

## Discussion

To add a toolbar item to the Finder, override the getter method for the toolbar image, name, and tooltip properties.

## See Also

### Managing Badges, Shortcut Menus, and Toolbar Buttons

func beginObservingDirectory(at: URL)

Tells the extension that the user is looking at a monitored directory or at one of its subdirectories.

func endObservingDirectory(at: URL)

Tells the extension that the user has stopped looking at a monitored directory or at one of its subdirectories.

func menu(for: FIMenuKind) -> NSMenu?

Requests a custom menu from the extension.

func requestBadgeIdentifier(for: URL)

Requests a badge for the given file or directory.

var toolbarItemName: String

The name of the extension’s toolbar button.

var toolbarItemToolTip: String

The tooltip text for the extension’s toolbar button.

