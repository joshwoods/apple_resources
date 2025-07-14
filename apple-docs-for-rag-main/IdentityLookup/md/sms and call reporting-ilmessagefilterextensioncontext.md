

- SMS and Call Reporting
-  ILMessageFilterExtensionContext 

Class

# ILMessageFilterExtensionContext

The extension context for a Message Filter app extension.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILMessageFilterExtensionContext
```

## Topics

### Deferring a Request to the Network

func deferQueryRequestToNetwork(completion: (ILNetworkResponse?, (any Error)?) -> Void)

Tells the system to pass the current query request to the app extension’s associated network service.

## Relationships

### Inherits From

- NSExtensionContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### App Extension

class ILMessageFilterExtension

The abstract base class for the principal class of a Message Filter app extension.

