

- AVFoundation
- AVPlayerLayer
-  isReadyForDisplay 

Instance Property

# isReadyForDisplay

A Boolean value that indicates whether the first video frame of the player’s current item is ready for display.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var isReadyForDisplay: Bool { get }
```

## Discussion

Use this property to determine when to show or animate a player layer into view. You can display a player layer while this property value is false, but the layer doesn’t present any content until the value becomes true.

This property remains false for a player when its currentItem contains no enabled video tracks.

This property is key-value observable.

