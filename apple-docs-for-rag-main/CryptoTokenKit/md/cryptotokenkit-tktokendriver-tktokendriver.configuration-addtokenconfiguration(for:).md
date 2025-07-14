

- CryptoTokenKit
- TKTokenDriver
- TKTokenDriver.Configuration
-  addTokenConfiguration(for:) 

Instance Method

# addTokenConfiguration(for:)

Creates a configuration object for a token with the token instance identifier you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func addTokenConfiguration(for instanceID: TKToken.InstanceID) -> TKToken.Configuration
```

## Parameters 

`instanceID`  

The token’s instance identifier.

## Return Value

The configuration class for the token.

## Discussion

This method adds the created configuration into the tokenConfigurations dictionary. Adding a configuration with an `instanceID` that already exists replaces the existing configuration with a new empty configuration.

## See Also

### Adding and Removing Configurations

func removeTokenConfiguration(for: TKToken.InstanceID)

Removes a configuration for a token with the token instance identifier you specify.

