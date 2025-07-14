

- Finder Sync
- FIFinderSyncController
-  setBadgeImage(\_:label:forBadgeIdentifier:) 

Instance Method

# setBadgeImage(\_:label:forBadgeIdentifier:)

Sets the badge image and label for the given ID.

macOS 10.10+

``` source
func setBadgeImage(
    _ image: NSImage,
    label: String?,
    forBadgeIdentifier badgeID: String
)
```

## Parameters 

`image`  

An NSImage object. The system may or may not draw this image on top of the item’s icon; when it does, the system determines the overlay position. Don’t add any padding to the image to adjust this positioning. The image draws at up to 320 x 320 points.

`label`  

A label describing the sync state represented by this badge. Each label should be a short localized string, such as “Waiting.”

`badgeID`  

A unique ID, identifying this badge.

## Discussion

Use this method to configure your badges. Finder may display the image, the label or both. Your Finder Sync extension typically sets up a fixed number of badges during its `init` method.

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

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

