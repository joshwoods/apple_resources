

- File Provider
- NSFileProviderRequest
-  requestingExecutable 

Instance Property

# requestingExecutable

The URL of the requesting executable.

macOS 11.0+

``` source
var requestingExecutable: URL? { get }
```

## Discussion

This property is `nil` unless the device has a Mobile Device Management (MDM) profile, and the profile’s administrator installed the file provider’s app using the MDM profile.

## See Also

### Accessing Application Information

var domainVersion: NSFileProviderDomainVersion?

The version of the domain for the request.

var isFileViewerRequest: Bool

A Boolean value that indicates whether the request came from Finder or related system file browsers.

var isSystemRequest: Bool

A Boolean value that indicates whether the request came from a system process.

