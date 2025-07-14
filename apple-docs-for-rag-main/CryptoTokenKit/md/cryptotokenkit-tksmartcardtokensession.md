

- CryptoTokenKit
-  TKSmartCardTokenSession 

Class

# TKSmartCardTokenSession

A token session that is based on a smart card token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKSmartCardTokenSession
```

## Mentioned in 

Authenticating Users with a Cryptographic Token

## Overview

You can use the smartCard property to access and send APDUs to the underlying smart card.

## Topics

### Accessing the Smart Card

var smartCard: TKSmartCard

The smart card for the active exclusive session and selected application.

## Relationships

### Inherits From

- TKTokenSession

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

class TKSmartCardTokenDriver

The driver that acts as an entry point for smart card app extensions.

class TKSmartCardToken

A representation of a smart card based cryptographic token.

