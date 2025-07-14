

- ShazamKit
- SHMatchedMediaItem
-  matchOffset 

Instance Property

# matchOffset

The timecode in the reference recording that matches the start of the query, in seconds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var matchOffset: TimeInterval { get }
```

## Discussion

The value can be negative if the query signature contains unrecognizable data before the data that corresponds to the start of the matched reference item.

## See Also

### Reading information about the match

var predictedCurrentMatchOffset: TimeInterval

The updated timecode in the reference recording that matches the current playback position of the query audio, in seconds.

var frequencySkew: Float

A multiple for the difference in frequency between the matched audio and the query audio.

