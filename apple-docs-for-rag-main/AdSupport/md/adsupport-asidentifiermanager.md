

- AdSupport
-  ASIdentifierManager 

Class

# ASIdentifierManager

The object that contains the advertising identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.14+tvOS 6.0+

``` source
class ASIdentifierManager
```

## Topics

### Getting the Advertising Identifier

class func shared() -> ASIdentifierManager

The shared instance of the identifier manager class.

var advertisingIdentifier: UUID

The UUID that is specific to a device.

### Deprecated

var isAdvertisingTrackingEnabled: Bool

A Boolean value that indicates whether the user has limited ad tracking enabled.

Deprecated

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

