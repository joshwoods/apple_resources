

- ShazamKit
- SHMatchedMediaItem
-  predictedCurrentMatchOffset 

Instance Property

# predictedCurrentMatchOffset

The updated timecode in the reference recording that matches the current playback position of the query audio, in seconds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var predictedCurrentMatchOffset: TimeInterval { get }
```

## Mentioned in 

Matching audio using the built-in microphone

## See Also

### Reading information about the match

var matchOffset: TimeInterval

The timecode in the reference recording that matches the start of the query, in seconds.

var frequencySkew: Float

A multiple for the difference in frequency between the matched audio and the query audio.

