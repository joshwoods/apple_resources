

- Create ML
- MLSoundClassifier
-  predictions(from:overlapFactor:predictionTimeWindowSize:) 

Instance Method

# predictions(from:overlapFactor:predictionTimeWindowSize:)

Generates predictions that use an overlap factor and time window size for an array of audio files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func predictions(
    from audioFiles: [URL],
    overlapFactor: Double,
    predictionTimeWindowSize: TimeInterval
) throws -> [String]
```

## Parameters 

`audioFiles`  

An array of audio-file URLs you want the sound classifier to categorize.

`overlapFactor`  

The amount of overlap between successive analysis windows when the model analyzes a block of audio data.

`predictionTimeWindowSize`  

The duration of the audio buffer the method sends to the model for each prediction.

## Return Value

An array of prediction labels for the audio files.

## See Also

### Testing a sound classifier

func predictions(from: [URL]) throws -> [String]

Generates predictions for an array of audio files.

