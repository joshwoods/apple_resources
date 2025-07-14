

- ShazamKit
- SHSignature
-  duration 

Instance Property

# duration

The duration of the audio you use to generate the signature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var duration: TimeInterval { get }
```

## Discussion

Audio that contains periods of silence may result in a duration value that’s shorter than the full duration of the original audio track.

## See Also

### Reading signature information

var dataRepresentation: Data

The raw data for the signature.

