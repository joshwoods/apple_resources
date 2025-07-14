

- CryptoTokenKit
- TKTokenDriver
- TKTokenDriver.Configuration
-  removeTokenConfiguration(for:) 

Instance Method

# removeTokenConfiguration(for:)

Removes a configuration for a token with the token instance identifier you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func removeTokenConfiguration(for instanceID: TKToken.InstanceID)
```

## Parameters 

`instanceID`  

The token’s instance identifier.

## Discussion

The method does nothing if the token configuration you specify doesn’t exist.

## See Also

### Adding and Removing Configurations

func addTokenConfiguration(for: TKToken.InstanceID) -> TKToken.Configuration

Creates a configuration object for a token with the token instance identifier you specify.

