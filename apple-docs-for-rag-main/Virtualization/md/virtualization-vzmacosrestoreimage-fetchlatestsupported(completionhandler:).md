

- Virtualization
- VZMacOSRestoreImage
-  fetchLatestSupported(completionHandler:) 

Type Method

# fetchLatestSupported(completionHandler:)

Fetches the latest restore image supported by this host from the network.

macOS 12.0+

``` source
class func fetchLatestSupported(completionHandler: @escaping (Result) -> Void)
```

## Parameters 

`completionHandler`  

A block called after the restore image fetch has succeeded or failed. The `error` parameter passed to the block is `nil` if the image restoration was successful.

The system invokes the completion handler on an arbitrary thread. The completion handler returns an `error` parameter that describes the reason for the failure; the block is `nil` if installation was successful.

## Discussion

Construct a VZMacOSInstaller object with a `VZMacOSRestoreImage` loaded from a file on the local file system. A `VZMacOSRestoreImage` fetched with the latestSupported method has a URL property that refers to a restore image on the network.

To use a network restore image, download the file to disk (using URLSession or similar API). After downloading the restore image, you can initialize a VZMacOSInstaller using a URL referring to the local file.

## See Also

### Controlling the Restoration Process

class func load(from: URL, completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Load a restore image from a file on the local file system.

class var latestSupported: VZMacOSRestoreImage

Fetches the latest restore image supported by this host from the network.

class func image(from: URL) async throws -> VZMacOSRestoreImage

Load a restore image from a file on the local file system.

