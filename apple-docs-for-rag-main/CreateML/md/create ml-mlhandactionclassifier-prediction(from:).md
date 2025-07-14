

- Create ML
- MLHandActionClassifier
-  prediction(from:) 

Instance Method

# prediction(from:)

Generates a hand action prediction for a video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func prediction(from video: URL) throws -> [MLHandActionClassifier.Prediction]
```

## Return Value

An array of predictions.

## See Also

### Testing a hand action classifier

func predictions(from: [URL]) throws -> [[MLHandActionClassifier.Prediction]]

Generates an array of hand action predictions for each video in a URL array.

struct Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

