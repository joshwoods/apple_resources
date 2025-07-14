

- AVFoundation
- AVAssetDownloadURLSession
-  init(configuration:assetDownloadDelegate:delegateQueue:) 

Initializer

# init(configuration:assetDownloadDelegate:delegateQueue:)

Creates a URL session to download assets.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
init(
    configuration: URLSessionConfiguration,
    assetDownloadDelegate delegate: (any AVAssetDownloadDelegate)?,
    delegateQueue: OperationQueue?
)
```

## Parameters 

`configuration`  

The configuration for this download session. The configuration you provide must be a *background* configuration or the system raises an exception.

`delegate`  

The delegate object to handle asset download progress updates and other session related events.

`delegateQueue`  

The queue to receive delegate callbacks on. If you specify `nil`, the system provides a serial queue.

## Return Value

A new download session.

## See Also

### Creating a Download Session

protocol AVAssetDownloadDelegate

A protocol that defines the methods to implement to respond to asset-download events.

