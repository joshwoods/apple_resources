

- Background Assets
-  BAURLDownload 

Class

# BAURLDownload

An object that represents a remote asset to download.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
class BAURLDownload
```

## Topics

### Creating a download

init(identifier: String, request: URLRequest, essential: Bool, fileSize: Int, applicationGroupIdentifier: String, priority: BADownload.Priority)

convenience init(identifier: String, request: URLRequest, fileSize: Int, applicationGroupIdentifier: String)

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String)

Creates a download that uses the specified identifier and App Group.

Deprecated

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String, priority: BADownload.Priority)

Creates a prioritized download that uses the specified identifier and App Group.

Deprecated

## Relationships

### Inherits From

- BADownload

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Asset downloads

class BADownload

An object that represents an in-progress or concluded asset download.

struct Priority

A type that determines the execution priority of a scheduled asset download.

