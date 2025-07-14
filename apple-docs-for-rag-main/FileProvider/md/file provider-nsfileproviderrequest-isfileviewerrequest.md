

- File Provider
- NSFileProviderRequest
-  isFileViewerRequest 

Instance Property

# isFileViewerRequest

A Boolean value that indicates whether the request came from Finder or related system file browsers.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
var isFileViewerRequest: Bool { get }
```

## See Also

### Accessing Application Information

var domainVersion: NSFileProviderDomainVersion?

The version of the domain for the request.

var requestingExecutable: URL?

The URL of the requesting executable.

var isSystemRequest: Bool

A Boolean value that indicates whether the request came from a system process.

