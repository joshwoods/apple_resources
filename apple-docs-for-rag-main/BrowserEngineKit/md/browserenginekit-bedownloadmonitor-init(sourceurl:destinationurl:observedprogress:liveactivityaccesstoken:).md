

- BrowserEngineKit
- BEDownloadMonitor
-  init(sourceURL:destinationURL:observedProgress:liveActivityAccessToken:) 

Initializer

# init(sourceURL:destinationURL:observedProgress:liveActivityAccessToken:)

Initializes a download monitor to report progress for the specified download.

iOS 18.2+iPadOS 18.2+

``` source
@objc(initWithSourceURL:destinationURL:observedProgress:liveActivityAccessToken:)
init(
    sourceURL: URL,
    destinationURL: URL,
    observedProgress: Progress,
    liveActivityAccessToken: Data
)
```

## Parameters 

`sourceURL`  

The location of the resource on the web that someone wants to download.

`destinationURL`  

The location of the file to which you save the resource.

`observedProgress`  

An object you use to report the download’s progress to the system.

`liveActivityAccessToken`  

An opaque token that the system checks to verify that your networking extension can remain active while the download is in progress.

## Discussion

Generate an access token for the download by calling createAccessToken().

## See Also

### Creating a download monitor

static func createAccessToken() -> Data?

Generates an opaque token that the system uses to keep your networking extension active in the background.

