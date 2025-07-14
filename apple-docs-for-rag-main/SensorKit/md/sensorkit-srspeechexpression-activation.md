

- SensorKit
- SRSpeechExpression
-  activation 

Instance Property

# activation

The level of energy or activation of the speaker.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var activation: Double { get }
```

## Discussion

This property is a range from `-1` to `1`, where negative values indicate negative sentiment, and positive values indicate positive sentiment.

## See Also

### Getting speech analytics

var confidence: Double

The level of confidence of the speaker.

var mood: Double

An indication of how slurry, tired, or exhausted the speaker sounds compared to normal speech.

var valence: Double

The degree of positive or negative emotion or sentiment of the speaker.

var dominance: Double

The degree of how strong or meek the speaker sounds.

