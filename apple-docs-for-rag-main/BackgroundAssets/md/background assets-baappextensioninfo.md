

- Background Assets
-  BAAppExtensionInfo 

Class

# BAAppExtensionInfo

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
class BAAppExtensionInfo
```

## Topics

### Getting the size of the remaining downloads

var restrictedEssentialDownloadSizeRemaining: Int?

var restrictedDownloadSizeRemaining: Int?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Checking for asset updates

func downloads(for: BAContentRequest, manifestURL: URL, extensionInfo: BAAppExtensionInfo) -> Set&lt;BADownload>

**Required** Default implementation provided.

enum BAContentRequest

