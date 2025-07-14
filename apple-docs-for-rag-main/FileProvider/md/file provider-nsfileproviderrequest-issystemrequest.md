

- File Provider
- NSFileProviderRequest
-  isSystemRequest 

Instance Property

# isSystemRequest

A Boolean value that indicates whether the request came from a system process.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
var isSystemRequest: Bool { get }
```

## Discussion

System requests occur, for example, when the system needs to update a file after receiving a push notification about a change from the remote storage.

## See Also

### Accessing Application Information

var domainVersion: NSFileProviderDomainVersion?

The version of the domain for the request.

var requestingExecutable: URL?

The URL of the requesting executable.

var isFileViewerRequest: Bool

A Boolean value that indicates whether the request came from Finder or related system file browsers.

