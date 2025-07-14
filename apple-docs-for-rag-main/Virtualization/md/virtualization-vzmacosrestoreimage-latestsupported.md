

- Virtualization
- VZMacOSRestoreImage
-  latestSupported 

Type Property

# latestSupported

Fetches the latest restore image supported by this host from the network.

macOS 12.0+

``` source
class var latestSupported: VZMacOSRestoreImage { get async throws }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

Construct a VZMacOSInstaller object with a `VZMacOSRestoreImage` loaded from a file on the local file system. A `VZMacOSRestoreImage` fetched with the latestSupported method has a URL property that refers to a restore image on the network.

To use a network restore image, download the file to disk (using URLSession or similar API). After downloading the restore image, you can initialize a VZMacOSInstaller using a URL referring to the local file.

## See Also

### Controlling the Restoration Process

class func fetchLatestSupported(completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Fetches the latest restore image supported by this host from the network.

class func load(from: URL, completionHandler: (Result&lt;VZMacOSRestoreImage, any Error>) -> Void)

Load a restore image from a file on the local file system.

class func image(from: URL) async throws -> VZMacOSRestoreImage

Load a restore image from a file on the local file system.

