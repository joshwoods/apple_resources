

- Apple CryptoKit
- HMAC
-  isValidAuthenticationCode(\_:authenticating:using:) 

Type Method

# isValidAuthenticationCode(\_:authenticating:using:)

Returns a Boolean value indicating whether the given message authentication code represented as contiguous bytes is valid for a block of data.

iOS 13.2+iPadOS 13.2+Mac Catalyst 13.2+macOS 10.15+tvOS 13.2+visionOS 1.0+watchOS 6.1+

``` source
static func isValidAuthenticationCode(
    _ authenticationCode: C,
    authenticating authenticatedData: D,
    using key: SymmetricKey
) -> Bool where C : ContiguousBytes, D : DataProtocol
```

## Parameters 

`authenticationCode`  

The authentication code to compare.

`authenticatedData`  

The block of data to compare.

`key`  

The symmetric key for the authentication code.

## Return Value

A Boolean value that’s `true` if the message authentication code is valid for the specified block of data.

## See Also

### Checking an authentication code

static func isValidAuthenticationCode&lt;D>(HMAC&lt;H>.MAC, authenticating: D, using: SymmetricKey) -> Bool

Returns a Boolean value indicating whether the given message authentication code is valid for a block of data.

static func isValidAuthenticationCode(HMAC&lt;H>.MAC, authenticating: UnsafeRawBufferPointer, using: SymmetricKey) -> Bool

Returns a Boolean value indicating whether the given message authentication code is valid for a block of data stored in a buffer.

