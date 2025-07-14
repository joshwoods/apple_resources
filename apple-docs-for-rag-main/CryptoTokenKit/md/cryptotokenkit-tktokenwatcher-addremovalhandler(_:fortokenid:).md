

- CryptoTokenKit
- TKTokenWatcher
-  addRemovalHandler(\_:forTokenID:) 

Instance Method

# addRemovalHandler(\_:forTokenID:)

Adds a removal handler for the specified token ID.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func addRemovalHandler(
    _ removalHandler: @escaping (String) -> Void,
    forTokenID tokenID: String
)
```

## Parameters 

`removalHandler`  

A block to be called when the specified token is removed. This block takes a single argument:

tokenID  
The identifier of the removed token.

`tokenID`  

The identifier of the token to watch for removal.

If tokenIDs doesn’t contain `tokenID`, `insertionHandler` is executed immediately.

## Mentioned in 

Using Cryptographic Assets Stored on a Smart Card

## Discussion

You typically call this method in the `insertionHandler` passed to the token watcher initializer.

Adding a removal handler will remove any existing removal handlers for the specified token ID.

## See Also

### Configuring Handlers

func setInsertionHandler((String) -> Void)

Sets an insertion handler closure to be called when a new token is inserted into the system.

