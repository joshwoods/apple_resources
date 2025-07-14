

- AVFoundation
- AVPlayerItemAccessLogEvent
-  observedBitrate 

Instance Property

# observedBitrate

The empirical throughput, in bits per second, across all media downloaded.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var observedBitrate: Double { get }
```

## Discussion

The property corresponds to “c-observed-bitrate”.

The value of this property is negative if unknown.

This property is not compatible with key-value observing.

## See Also

### Getting Bit Rate Log Events

var observedBitrateStandardDeviation: Double

The standard deviation of the observed segment download bit rates.

var observedMaxBitrate: Double

The maximum observed segment download bit rate.

Deprecated

var observedMinBitrate: Double

The minimum observed segment download bit rate.

Deprecated

var switchBitrate: Double

The bandwidth value that causes a switch, up or down, in the item’s quality being played.

var indicatedBitrate: Double

The throughput, in bits per second, required to play the stream, as advertised by the server.

var averageAudioBitrate: Double

The audio track’s average bit rate, in bits per second.

var averageVideoBitrate: Double

The video track’s average bit rate, in bits per second.

var indicatedAverageBitrate: Double

The average throughput, in bits per second, required to play the stream, as advertised by the server.

