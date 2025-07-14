

- Finder Sync
- FIFinderSyncController
-  setBadgeIdentifier(\_:for:) 

Instance Method

# setBadgeIdentifier(\_:for:)

Sets the badge for a file or directory.

macOS 10.10+

``` source
func setBadgeIdentifier(
    _ badgeID: String,
    for url: URL
)
```

## Parameters 

`badgeID`  

A unique ID, identifying the badge.

`url`  

The URL of the file or directory.

## Discussion

Adds the specified badge to the given file or directory. Setting the identifier to an empty string (`@""`) removes the badge.

Avoid adding badges to items that the Finder hasn’t displayed yet. When setting the initial badge, call this method from your Finder Sync extension’s requestBadgeIdentifier(for:) method. When updating badges, call this method only for items that have already received a badge.

## See Also

### Related Documentation

func requestBadgeIdentifier(for: URL)

Requests a badge for the given file or directory.

### Managing the Finder Sync Controller

class func `default`() -> Self

Returns the shared Finder Sync controller object.

var directoryURLs: Set&lt;URL>!

The directories managed by this extension.

func selectedItemURLs() -> [URL]?

Returns an array of selected items.

func setBadgeImage(NSImage, label: String?, forBadgeIdentifier: String)

Sets the badge image and label for the given ID.

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

