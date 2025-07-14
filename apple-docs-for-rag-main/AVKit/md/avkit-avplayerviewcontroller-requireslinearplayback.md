

- AVKit
- AVPlayerViewController
-  requiresLinearPlayback 

Instance Property

# requiresLinearPlayback

A Boolean value that determines whether the player allows the user to skip media content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var requiresLinearPlayback: Bool { get set }
```

## Mentioned in 

Working with Interstitial Content

Adopting Picture in Picture in a Standard Player

## Discussion

If this value is false (the default), the controller’s user interface allows a user to fast-forward, scrub, or skip ahead to content later in the player’s presentation. To prevent the user from skipping content—for example, while presenting a legal notice or other mandatory interstitial content—set this property’s value to true.

To track when the player is presenting content for which you might require linear playback, use the interstitialTimeRanges property of the view controller’s player item to define the time ranges of the interstitial content. The view controller then sends playerViewController(_:willPresent:) and playerViewController(_:didPresent:) messages to its delegate object when the content is playing. Implement these methods to enable or disable the requiresLinearPlayback property as needed.

