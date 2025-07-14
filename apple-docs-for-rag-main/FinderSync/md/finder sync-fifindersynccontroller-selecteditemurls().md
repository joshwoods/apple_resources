

- Finder Sync
- FIFinderSyncController
-  selectedItemURLs() 

Instance Method

# selectedItemURLs()

Returns an array of selected items.

macOS 10.10+

``` source
func selectedItemURLs() -> [URL]?
```

## Return Value

An array of items currently selected in the Finder window.

## Discussion

Use this method when creating a shortcut menu or a menu for the extension’s toolbar button. You can then modify the menu’s content based on the items currently selected.

This method returns valid values only from the Finder Sync extension’s menu(for:) method or from one of the menu actions created in this method. If the selected items are outside the extension’s managed directories (for example, when the user clicks on the toolbar button), this method returns `nil`.

## See Also

### Managing the Finder Sync Controller

class func `default`() -> Self

Returns the shared Finder Sync controller object.

var directoryURLs: Set&lt;URL>!

The directories managed by this extension.

func setBadgeIdentifier(String, for: URL)

Sets the badge for a file or directory.

func setBadgeImage(NSImage, label: String?, forBadgeIdentifier: String)

Sets the badge image and label for the given ID.

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

