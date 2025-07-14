

- BrowserEngineKit
- BEDownloadMonitor
-  createAccessToken() 

Type Method

# createAccessToken()

Generates an opaque token that the system uses to keep your networking extension active in the background.

iOS 18.2+iPadOS 18.2+

``` source
@objc(createAccessToken)
static func createAccessToken() -> Data?
```

## Discussion

Use this method to generate a token that you pass to init(sourceURL:destinationURL:observedProgress:liveActivityAccessToken:).

## See Also

### Creating a download monitor

init(sourceURL: URL, destinationURL: URL, observedProgress: Progress, liveActivityAccessToken: Data)

Initializes a download monitor to report progress for the specified download.

