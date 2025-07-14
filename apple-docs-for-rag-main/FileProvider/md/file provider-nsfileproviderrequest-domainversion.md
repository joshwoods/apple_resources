

- File Provider
- NSFileProviderRequest
-  domainVersion 

Instance Property

# domainVersion

The version of the domain for the request.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var domainVersion: NSFileProviderDomainVersion? { get }
```

## Discussion

If the file provider extension doesn’t implement the NSFileProviderDomainState protocol, this property is `nil`.

## See Also

### Accessing Application Information

var requestingExecutable: URL?

The URL of the requesting executable.

var isFileViewerRequest: Bool

A Boolean value that indicates whether the request came from Finder or related system file browsers.

var isSystemRequest: Bool

A Boolean value that indicates whether the request came from a system process.

