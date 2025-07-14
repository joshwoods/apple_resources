

- CryptoTokenKit
- TKTokenWatcher
-  setInsertionHandler(\_:) 

Instance Method

# setInsertionHandler(\_:)

Sets an insertion handler closure to be called when a new token is inserted into the system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func setInsertionHandler(_ insertionHandler: @escaping (String) -> Void)
```

## Parameters 

`insertionHandler`  

A closure to be called whenever a token is added to the system. The closure takes a single argument, the tokenID, that identifies the added token.

## Mentioned in 

Using Cryptographic Assets Stored on a Smart Card

## See Also

### Configuring Handlers

func addRemovalHandler((String) -> Void, forTokenID: String)

Adds a removal handler for the specified token ID.

