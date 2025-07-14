

- Link Presentation
-  LPLinkMetadata 

Class

# LPLinkMetadata

An object that contains metadata about a URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class LPLinkMetadata
```

## Overview

Use LPLinkMetadata to store the metadata about a URL, including its title, icon, images and video.

Fetch metadata using LPMetadataProvider. For remote URLs, cache the metadata locally to avoid the data and performance cost of fetching it from the internet every time you present it. LPLinkMetadata is serializable with NSSecureCoding.

For local file URLs, the Quick Look Thumbnailing API retrieves a representative thumbnail for the file, if possible.

## Provide custom metadata

Say your app already has a database of links, with titles and images that weren’t fetched by LPMetadataProvider. You don’t have to fetch new metadata from the internet in order to accelerate the share sheet or to present a rich link. Instead, you can fill in the fields of LPLinkMetadata yourself.

Create an LPLinkMetadata object, and fill in at least the originalURL and url fields, plus whatever additional information you have.

```
```

## Accelerate the share sheet preview

For existing apps that share URLs, the share sheet automatically presents a preview of the link. The preview first shows a placeholder link icon alongside the base URL while fetching the link’s metadata over the network. The preview updates once the link’s icon and title become available.

If you already have an LPLinkMetadata object for a URL, pass it to the share sheet to present the preview instantly, without fetching data over the network. In your implementation of activityViewControllerLinkMetadata(_:), return the metadata object.

```
```

If the user chooses to share to Messages, the same metadata passes directly through, providing a smooth and seamless experience with no unnecessary loading.

## Topics

### Identifying the link

var url: URL?

The URL that returned the metadata, taking server-side redirects into account.

var originalURL: URL?

The original URL of the metadata request.

### Getting the link’s title

var title: String?

A representative title for the URL.

### Getting the link’s images

var iconProvider: NSItemProvider?

An object that retrieves data corresponding to a representative icon for the URL.

var imageProvider: NSItemProvider?

An object that retrieves data corresponding to a representative image for the URL.

### Getting the link’s video

var remoteVideoURL: URL?

A remote URL corresponding to a representative video for the URL.

var videoProvider: NSItemProvider?

An object that retrieves data corresponding to a representative video for the URL.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Link metadata

class LPMetadataProvider

An object that retrieves metadata for a URL.

