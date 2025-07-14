

- Virtualization
- VZMacOSRestoreImage
-  image(from:) 

Type Method

# image(from:)

Load a restore image from a file on the local file system.

macOS 12.0+

``` source
class func image(from fileURL: URL) async throws -> VZMacOSRestoreImage
```

## Parameters 

`fileURL`  

A file URL that indicates the macOS restore image to load.

## Discussion

`VZMacOSRestoreImage` can load macOS installation media from a local file. If the `fileURL` parameter doesn’t refer to a local file, the system raises an exception.

## See Also

### Controlling the Restoration Process

class func fetchLatestSupported(completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Fetches the latest restore image supported by this host from the network.

class func load(from: URL, completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Load a restore image from a file on the local file system.

class var latestSupported: VZMacOSRestoreImage

Fetches the latest restore image supported by this host from the network.

