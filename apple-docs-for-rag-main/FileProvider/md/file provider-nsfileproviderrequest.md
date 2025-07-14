

- File Provider
-  NSFileProviderRequest 

Class

# NSFileProviderRequest

An object that provides information about the application requesting data from the File Provider extension.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
class NSFileProviderRequest
```

## Topics

### Accessing Application Information

var domainVersion: NSFileProviderDomainVersion?

The version of the domain for the request.

var requestingExecutable: URL?

The URL of the requesting executable.

var isFileViewerRequest: Bool

A Boolean value that indicates whether the request came from Finder or related system file browsers.

var isSystemRequest: Bool

A Boolean value that indicates whether the request came from a system process.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Items and metadata

struct NSFileProviderItemFields

Fields that specify which of the item’s properties have changed.

class NSFileProviderItemVersion

The version of the item’s content and its metadata.

protocol NSFileProviderItemDecorating

Support for decorating items.

struct NSFileProviderItemDecorationIdentifier

A decoration identifier defined in the File Provider extension’s information property list.

