

- CryptoTokenKit
-  TKSmartCardTokenDriver 

Class

# TKSmartCardTokenDriver

The driver that acts as an entry point for smart card app extensions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKSmartCardTokenDriver
```

## Mentioned in 

Authenticating Users with a Cryptographic Token

## Topics

### Responding to Token Creation

protocol TKSmartCardTokenDriverDelegate

The interface that a smart card token driver delegate implements to respond to token creation events.

## Relationships

### Inherits From

- TKTokenDriver

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Smart Card App Extensions

Authenticating Users with a Cryptographic Token

Grant access to user accounts and the keychain by creating a smart card app extension.

Configuring Smart Card Authentication

Set preferences for smart card authentication operations, including those on managed devices.

class TKSmartCardToken

A representation of a smart card based cryptographic token.

class TKSmartCardTokenSession

A token session that is based on a smart card token.

