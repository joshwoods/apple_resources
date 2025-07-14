

- CryptoTokenKit
- TKToken
-  init(tokenDriver:instanceID:) 

Initializer

# init(tokenDriver:instanceID:)

Initializes a token with the driver you specify.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    tokenDriver: TKTokenDriver,
    instanceID: TKToken.InstanceID
)
```

## Parameters 

`tokenDriver`  

The driver of the token.

`instanceID`  

A unique, persistent identifier for this token. This value is typically generated from the serial number of the target hardware.

## Return Value

A new token object.

## Discussion

This is the designated initializer.

## See Also

### Creating Tokens

typealias InstanceID

A type that represents the instance identifier of a token.

