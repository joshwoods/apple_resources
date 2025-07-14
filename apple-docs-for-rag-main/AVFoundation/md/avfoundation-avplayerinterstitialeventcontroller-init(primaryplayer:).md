

- AVFoundation
- AVPlayerInterstitialEventController
-  init(primaryPlayer:) 

Initializer

# init(primaryPlayer:)

Creates an event controller with a player item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(primaryPlayer: AVPlayer)
```

## Parameters 

`primaryPlayer`  

A player that plays primary content. The system raises an exception you specify an interstitial player for this argument.

