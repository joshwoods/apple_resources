

- CryptoTokenKit
- TKTokenWatcher
-  tokenIDs 

Instance Property

# tokenIDs

The token IDs currently available in the system.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var tokenIDs: [String] { get }
```

## Mentioned in 

Using Cryptographic Assets Stored on a Smart Card

## Discussion

Each string in tokenIDs corresponds to the name of the token instance.

You can observe this property to be notified of additions and removals to system tokens. See Key-Value Observing Programming Guide for more information.

