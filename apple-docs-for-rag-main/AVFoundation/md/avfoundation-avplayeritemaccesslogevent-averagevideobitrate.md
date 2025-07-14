

- AVFoundation
- AVPlayerItemAccessLogEvent
-  averageVideoBitrate 

Instance Property

# averageVideoBitrate

The video track’s average bit rate, in bits per second.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var averageVideoBitrate: Double { get }
```

## Discussion

The property corresponds to “c-avg-video-bitrate”.

This property returns the average bitrate of the video track if it is unmuxed, or the average bitrate of the combined content if muxed. Measured in bits per second.

The value is negative if unknown.

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

var observedBitrate: Double

The empirical throughput, in bits per second, across all media downloaded.

var averageAudioBitrate: Double

The audio track’s average bit rate, in bits per second.

var indicatedAverageBitrate: Double

The average throughput, in bits per second, required to play the stream, as advertised by the server.

