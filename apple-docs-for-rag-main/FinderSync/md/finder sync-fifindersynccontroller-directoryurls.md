

- Finder Sync
- FIFinderSyncController
-  directoryURLs 

Instance Property

# directoryURLs

The directories managed by this extension.

macOS 10.10+

``` source
var directoryURLs: Set! { get set }
```

## Discussion

The extension receives beginObservingDirectory(at:) and endObservingDirectory(at:) messages for every directory in this set and for all of their subdirectories.

Always set `directoryURLs` when the extension starts. If there are no directories to watch, set `directoryURLs` to an empty set.

## See Also

### Managing the Finder Sync Controller

class func `default`() -> Self

Returns the shared Finder Sync controller object.

func selectedItemURLs() -> [URL]?

Returns an array of selected items.

func setBadgeIdentifier(String, for: URL)

Sets the badge for a file or directory.

func setBadgeImage(NSImage, label: String?, forBadgeIdentifier: String)

Sets the badge image and label for the given ID.

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

