

- Apple CryptoKit
- HMAC
-  isValidAuthenticationCode(\_:authenticating:using:) 

Type Method

# isValidAuthenticationCode(\_:authenticating:using:)

Returns a Boolean value indicating whether the given message authentication code is valid for a block of data stored in a buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func isValidAuthenticationCode(
    _ mac: HMAC.MAC,
    authenticating bufferPointer: UnsafeRawBufferPointer,
    using key: SymmetricKey
) -> Bool
```

## Parameters 

`mac`  

The authentication code to compare.

`bufferPointer`  

A pointer to the block of data to compare.

`key`  

The symmetric key for the authentication code.

## Return Value

A Boolean value that’s `true` if the message authentication code is valid for the data within the specified buffer.

## See Also

### Checking an authentication code

static func isValidAuthenticationCode&lt;D>(HMAC&lt;H>.MAC, authenticating: D, using: SymmetricKey) -> Bool

Returns a Boolean value indicating whether the given message authentication code is valid for a block of data.

static func isValidAuthenticationCode&lt;C, D>(C, authenticating: D, using: SymmetricKey) -> Bool

Returns a Boolean value indicating whether the given message authentication code represented as contiguous bytes is valid for a block of data.

