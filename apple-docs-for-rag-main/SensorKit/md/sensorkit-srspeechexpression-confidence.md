

- SensorKit
- SRSpeechExpression
-  confidence 

Instance Property

# confidence

The level of confidence of the speaker.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var confidence: Double { get }
```

## Discussion

This property is a range from `0` to `1`, where `1` indicates the most confident.

## See Also

### Getting speech analytics

var mood: Double

An indication of how slurry, tired, or exhausted the speaker sounds compared to normal speech.

var valence: Double

The degree of positive or negative emotion or sentiment of the speaker.

var activation: Double

The level of energy or activation of the speaker.

var dominance: Double

The degree of how strong or meek the speaker sounds.

