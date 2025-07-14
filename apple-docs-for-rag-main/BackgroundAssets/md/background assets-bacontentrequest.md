

- Background Assets
-  BAContentRequest 

Enumeration

# BAContentRequest

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum BAContentRequest
```

## Topics

### Content request types

case install

case periodic

case update

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking for asset updates

func downloads(for: BAContentRequest, manifestURL: URL, extensionInfo: BAAppExtensionInfo) -> Set&lt;BADownload>

**Required** Default implementation provided.

class BAAppExtensionInfo

