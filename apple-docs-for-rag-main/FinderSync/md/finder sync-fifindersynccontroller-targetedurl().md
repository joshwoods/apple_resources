

- Finder Sync
- FIFinderSyncController
-  targetedURL() 

Instance Method

# targetedURL()

Returns the URL of the Finder’s current target.

macOS 10.10+

``` source
func targetedURL() -> URL?
```

## Return Value

The URL of the Finder’s current target.

## Discussion

Use this method when creating a custom shortcut menu for the Finder. This returns the URL of the item that the user Control-clicked, letting you customize the menu for that item.

This method returns valid values only from the Finder Sync extension’s menu(for:) method or from one of the menu actions created in this method. If the selected items are outside the extension’s managed directories (for example, when the user clicks on the toolbar button), this method returns `nil`.

## See Also

### Managing the Finder Sync Controller

class func `default`() -> Self

Returns the shared Finder Sync controller object.

var directoryURLs: Set&lt;URL>!

The directories managed by this extension.

func selectedItemURLs() -> [URL]?

Returns an array of selected items.

func setBadgeIdentifier(String, for: URL)

Sets the badge for a file or directory.

func setBadgeImage(NSImage, label: String?, forBadgeIdentifier: String)

Sets the badge image and label for the given ID.

