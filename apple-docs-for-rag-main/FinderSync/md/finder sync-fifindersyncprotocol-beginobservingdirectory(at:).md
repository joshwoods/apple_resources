

- Finder Sync
- FIFinderSyncProtocol
-  beginObservingDirectory(at:) 

Instance Method

# beginObservingDirectory(at:)

Tells the extension that the user is looking at a monitored directory or at one of its subdirectories.

macOS 10.10+

``` source
optional func beginObservingDirectory(at url: URL)
```

## Parameters 

`url`  

The URL of the directory.

## Discussion

Override this method to receive notifications when the user opens the contents of a monitored directory or one of its subdirectories in the Finder. The system calls `beginObservingDirectoryAtURL:` only once for each unique URL. As long as the content remains visible in at least one Finder window, any additional Finder windows that open to the same URL are ignored.

Note

The system creates additional instances of your extension for any Open and Save dialogs. These extensions receive their own calls to `beginObservingDirectoryAtURL:`, even if the directory is already open in a Finder window.

## See Also

### Managing Badges, Shortcut Menus, and Toolbar Buttons

func endObservingDirectory(at: URL)

Tells the extension that the user has stopped looking at a monitored directory or at one of its subdirectories.

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

