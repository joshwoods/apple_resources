

- CryptoTokenKit
- TKTokenDriverDelegate
-  tokenDriver(\_:tokenFor:) 

Instance Method

# tokenDriver(\_:tokenFor:)

Creates a new token for the configuration you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
optional func tokenDriver(
    _ driver: TKTokenDriver,
    tokenFor configuration: TKToken.Configuration
) throws -> TKToken
```

## Parameters 

`driver`  

The token driver.

`configuration`  

The configuration that identifies the token to create.

## Return Value

The created token.

## Discussion

The system invokes this method to request creation of a token instance, which the instanceID property of the configuration you specify identifies.

The created token has access to its current configuration using the configurationData property, which can provide token-implementation-specific additional data. The token can access keychain items this token exports with the methods key(for:) and certificate(for:) that the configuration provides.

Note

Smart card token drivers must not implement this method.

## See Also

### Creating and Removing Tokens

func tokenDriver(TKTokenDriver, terminateToken: TKToken)

Tells the delegate to terminate the token you specify.

