

- ShazamKit
- SHMatchedMediaItem
-  frequencySkew 

Instance Property

# frequencySkew

A multiple for the difference in frequency between the matched audio and the query audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var frequencySkew: Float { get }
```

## Discussion

A value of `0.0` indicates that the query and matched audio are at the same frequency. Other values indicate that the query audio is playing at a different frequency. For example, if the original recording plays at `100` Hz, a value of `0.05` indicates that the query recording plays at `105` Hz.

No match returns if the frequency skew is too large.

## See Also

### Reading information about the match

var matchOffset: TimeInterval

The timecode in the reference recording that matches the start of the query, in seconds.

var predictedCurrentMatchOffset: TimeInterval

The updated timecode in the reference recording that matches the current playback position of the query audio, in seconds.

