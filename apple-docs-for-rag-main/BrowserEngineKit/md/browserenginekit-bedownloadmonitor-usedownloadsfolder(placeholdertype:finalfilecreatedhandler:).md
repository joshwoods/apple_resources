

- BrowserEngineKit
- BEDownloadMonitor
-  useDownloadsFolder(placeholderType:finalFileCreatedHandler:) 

Instance Method

# useDownloadsFolder(placeholderType:finalFileCreatedHandler:)

Asks the system to create a placeholder for the downloaded file in the person’s Downloads folder.

iOS 18.2+iPadOS 18.2+

``` source
@objc(useDownloadsFolderWithPlaceholderType:finalFileCreatedHandler:)
func useDownloadsFolder(
    placeholderType: UTType? = nil,
    finalFileCreatedHandler: @escaping (BEDownloadMonitor.Location?) -> Void
)
```

## Parameters 

`placeholderType`  

The type of the file for which the system creates a placeholder. If this is `nil`, the system chooses a type based on the download’s filename extension.

`finalFileCreatedHandler`  

A closure you use to receive the location of the downloaded file in the person’s Downloads folder.

## Mentioned in 

Downloading files in a web browser with an alternative browser engine

## See Also

### Creating a download placeholder

class Location

A class that associates a URL with the bookmark you use to access that URL.

