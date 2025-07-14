

- Foundation
- URLUbiquitousItemDownloadingStatus
-  current 

Type Property

# current

A local copy of this item exists and is the most up-to-date version known to the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let current: URLUbiquitousItemDownloadingStatus
```

## See Also

### Constants

static let downloaded: URLUbiquitousItemDownloadingStatus

A local copy of this item exists, but it is stale. The most recent version will be downloaded as soon as possible.

static let notDownloaded: URLUbiquitousItemDownloadingStatus

This item has not been downloaded yet. Use startDownloadingUbiquitousItem(at:) to download it.

