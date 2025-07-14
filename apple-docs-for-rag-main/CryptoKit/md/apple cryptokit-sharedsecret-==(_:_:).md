

- Apple CryptoKit
- SharedSecret
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Determines whether a shared secret is equivalent to a collection of contiguous bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: SharedSecret, rhs: D) -> Bool where D : DataProtocol
```

## Parameters 

`lhs`  

The shared secret to compare.

`rhs`  

A collection of contiguous bytes to compare.

## Return Value

A Boolean value that’s `true` if the shared secret and the collection of binary data are equivalent.

