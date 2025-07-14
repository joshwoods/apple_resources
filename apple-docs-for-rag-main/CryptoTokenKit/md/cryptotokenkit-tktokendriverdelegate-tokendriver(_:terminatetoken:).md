

- CryptoTokenKit
- TKTokenDriverDelegate
-  tokenDriver(\_:terminateToken:) 

Instance Method

# tokenDriver(\_:terminateToken:)

Tells the delegate to terminate the token you specify.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func tokenDriver(
    _ driver: TKTokenDriver,
    terminateToken token: TKToken
)
```

## Parameters 

`driver`  

The token driver.

`token`  

The token to be terminated.

## See Also

### Creating and Removing Tokens

func tokenDriver(TKTokenDriver, tokenFor: TKToken.Configuration) throws -> TKToken

Creates a new token for the configuration you specify.

