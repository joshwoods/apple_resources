

- Media Player
- MPSkipIntervalCommand
-  preferredIntervals 

Instance Property

# preferredIntervals

The available skip intervals, in seconds, for a media item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var preferredIntervals: [NSNumber] { get set }
```

## Discussion

The `preferredIntervals` property holds an array of TimeInterval objects that designate different skip intervals for a media item. The skip intervals are defined in seconds.

