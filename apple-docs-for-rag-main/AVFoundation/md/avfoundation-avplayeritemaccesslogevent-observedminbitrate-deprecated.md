

- AVFoundation
- AVPlayerItemAccessLogEvent
-  observedMinBitrate Deprecated

Instance Property

# observedMinBitrate

The minimum observed segment download bit rate.

iOS 7.0–15.0DeprecatediPadOS 7.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.9–12.0DeprecatedtvOS 9.0–15.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
var observedMinBitrate: Double { get }
```

Deprecated

Use observedBitrateStandardDeviation to monitor variance in network bitrate.

## Discussion

The value of the property is negative if unknown.

Corresponds to “c-observed-min-bitrate”.

This property is not compatible with key-value observing.

## See Also

### Getting Bit Rate Log Events

var observedBitrateStandardDeviation: Double

The standard deviation of the observed segment download bit rates.

var observedMaxBitrate: Double

The maximum observed segment download bit rate.

Deprecated

var switchBitrate: Double

The bandwidth value that causes a switch, up or down, in the item’s quality being played.

var indicatedBitrate: Double

The throughput, in bits per second, required to play the stream, as advertised by the server.

var observedBitrate: Double

The empirical throughput, in bits per second, across all media downloaded.

var averageAudioBitrate: Double

The audio track’s average bit rate, in bits per second.

var averageVideoBitrate: Double

The video track’s average bit rate, in bits per second.

var indicatedAverageBitrate: Double

The average throughput, in bits per second, required to play the stream, as advertised by the server.

