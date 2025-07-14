

- Virtualization
- VZMacOSRestoreImage
-  load(from:completionHandler:) 

Type Method

# load(from:completionHandler:)

Load a restore image from a file on the local file system.

macOS 12.0+

``` source
class func load(
    from fileURL: URL,
    completionHandler: @escaping (Result) -> Void
)
```

## Parameters 

`fileURL`  

A file URL that indicates the macOS restore image to load.

`completionHandler`  

A block called after the restore image successfully loaded or has failed to load. The `error` parameter passed to the block is `nil` if the restore image loads successfully.

The system invokes the completion handler on an arbitrary thread.

## Discussion

`VZMacOSRestoreImage` can load macOS installation media from a local file. If the `fileURL` parameter doesn’t refer to a local file, the system raises an exception.

## See Also

### Controlling the Restoration Process

class func fetchLatestSupported(completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Fetches the latest restore image supported by this host from the network.

class var latestSupported: VZMacOSRestoreImage

Fetches the latest restore image supported by this host from the network.

class func image(from: URL) async throws -> VZMacOSRestoreImage

Load a restore image from a file on the local file system.

