

- StoreKit
- SKOverlayDelegate
-  storeOverlayDidFailToLoad(\_:error:) 

Instance Method

# storeOverlayDidFailToLoad(\_:error:)

Indicates that an overlay failed to load.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
optional func storeOverlayDidFailToLoad(
    _ overlay: SKOverlay,
    error: any Error
)
```

## Parameters 

`overlay`  

An overlay object that failed to load.

`error`  

An indication of why the overlay failed to load.

## Discussion

Common cases for a failure when loading an overlay are:

- Using invalid iTunes identifiers.

- Trying to present an overlay for media that’s not an app.

- Trying to present an overlay from an app extension or the simulator.

