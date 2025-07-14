

- BrowserEngineKit
- BEDownloadMonitor
-  BEDownloadMonitor.Location 

Class

# BEDownloadMonitor.Location

A class that associates a URL with the bookmark you use to access that URL.

iOS 18.2+iPadOS 18.2+

``` source
@objc(BEDownloadMonitorLocation)
class Location
```

## Discussion

Pass the bookmarkData to your browser app to resolve the URL in the app. For information on using XPC to share data between your networking extension and browser app, see Using XPC to communicate with browser extensions.

The URL bookmark in a `Location` isn’t suitable for storing on disk and resolving in subsequent launches of your app. To do this, create your own bookmark using bookmarkDataWithOptions:includingResourceValuesForKeys:relativeToURL:error:, passing the withSecurityScope flag.

## Topics

### Getting information about a location

let url: URL

The location of the resource.

let bookmarkData: Data

A bookmark that resolves to the resource’s URL.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Creating a download placeholder

func useDownloadsFolder(placeholderType: UTType?, finalFileCreatedHandler: (BEDownloadMonitor.Location?) -> Void)

Asks the system to create a placeholder for the downloaded file in the person’s Downloads folder.

