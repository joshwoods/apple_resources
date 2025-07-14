

- Create ML
- MLSoundClassifier
-  predictions(from:) 

Instance Method

# predictions(from:)

Generates predictions for an array of audio files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
func predictions(from audioFiles: [URL]) throws -> [String]
```

## Parameters 

`audioFiles`  

An array of audio-file URLs you want the sound classifier to categorize.

## Return Value

An array of prediction labels for the audio files.

## See Also

### Testing a sound classifier

func predictions(from: [URL], overlapFactor: Double, predictionTimeWindowSize: TimeInterval) throws -> [String]

Generates predictions that use an overlap factor and time window size for an array of audio files.

