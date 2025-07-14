

- Finder Sync
- FIFinderSyncController
-  default() 

Type Method

# default()

Returns the shared Finder Sync controller object.

macOS 10.10+

``` source
class func `default`() -> Self
```

## Return Value

The default Finder Sync controller object for this extension.

## See Also

### Managing the Finder Sync Controller

var directoryURLs: Set&lt;URL>!

The directories managed by this extension.

func selectedItemURLs() -> [URL]?

Returns an array of selected items.

func setBadgeIdentifier(String, for: URL)

Sets the badge for a file or directory.

func setBadgeImage(NSImage, label: String?, forBadgeIdentifier: String)

Sets the badge image and label for the given ID.

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

