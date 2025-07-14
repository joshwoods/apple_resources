

- CryptoTokenKit
- TKToken
-  configuration 

Instance Property

# configuration

The current configuration for a token.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var configuration: TKToken.Configuration { get }
```

## Discussion

Access keychain items exported by this token with the methods key(for:) and certificate(for:) provided by the configuration. You can access token-implementation-specific additional data using the configurationData property of the configuration.

## See Also

### Configuring the Token

class Configuration

A token’s configuration.

