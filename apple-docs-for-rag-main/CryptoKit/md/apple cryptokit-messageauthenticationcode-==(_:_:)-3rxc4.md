

- Apple CryptoKit
- MessageAuthenticationCode
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether a message authentication code is equivalent to a collection of binary data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Self, rhs: D) -> Bool where D : DataProtocol
```

## Parameters 

`lhs`  

A message authentication code to compare.

`rhs`  

A collection of binary data to compare.

## Return Value

A Boolean value that’s `true` if the message authentication code and the collection of binary data are equivalent.

## See Also

### Comparing codes

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two message authentication codes are equal.

