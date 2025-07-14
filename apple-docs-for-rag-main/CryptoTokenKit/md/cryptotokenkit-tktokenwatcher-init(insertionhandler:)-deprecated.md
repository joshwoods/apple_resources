

- CryptoTokenKit
- TKTokenWatcher
-  init(insertionHandler:) Deprecated

Initializer

# init(insertionHandler:)

Initializes a token watcher with the specified insertion handler.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.13DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
init(insertionHandler: @escaping (String) -> Void)
```

Deprecated

Use init() followed by a call to setInsertionHandler(_:) instead.

## Parameters 

`insertionHandler`  

A block to be called each time a token is added. This block takes a single argument:

tokenID  
The identifier of the added token.

## Return Value

A new token watcher object.

## Discussion

This is the designated initializer.

## See Also

### Creating Token Watchers

init()

Initializes a token watcher.

