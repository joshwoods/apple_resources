

- Foundation
- URLUbiquitousItemDownloadingStatus
-  notDownloaded 

Type Property

# notDownloaded

This item has not been downloaded yet. Use startDownloadingUbiquitousItem(at:) to download it.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let notDownloaded: URLUbiquitousItemDownloadingStatus
```

## See Also

### Constants

static let current: URLUbiquitousItemDownloadingStatus

A local copy of this item exists and is the most up-to-date version known to the device.

static let downloaded: URLUbiquitousItemDownloadingStatus

A local copy of this item exists, but it is stale. The most recent version will be downloaded as soon as possible.

