

- CryptoTokenKit
- TKToken
-  TKToken.Configuration 

Class

# TKToken.Configuration

A token’s configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class Configuration
```

## Overview

When you introduce a new TKToken.Configuration into the system, it can inform the system about its identities, consisting of both private keys and certificates, which the keychainItems property provides. Use the configurationData property to set additional configuration data.

You configure always-available tokens on a per-user basis. Although the token driver and the app hosting the token extension are shared across the system, the configuration for a token is stored individually for each user.

## Topics

### Reporting Configuration Information

var instanceID: TKToken.InstanceID

The unique, persistent identifier of this token that the token implementation creates.

var configurationData: Data?

Additional configuration information for the token instance.

### Retrieving Keys and Certificates

var keychainItems: [TKTokenKeychainItem]

The keychain items associated with this token.

func certificate(for: TKToken.ObjectID) throws -> TKTokenKeychainCertificate

Returns a certificate from the keychain with the object identifier you specify.

func key(for: TKToken.ObjectID) throws -> TKTokenKeychainKey

Returns a key from the keychain with the object identifier you specify.

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

### Configuring the Token

var configuration: TKToken.Configuration

The current configuration for a token.

