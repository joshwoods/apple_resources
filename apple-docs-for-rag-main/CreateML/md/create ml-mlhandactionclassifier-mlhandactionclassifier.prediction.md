

- Create ML
- MLHandActionClassifier
-  MLHandActionClassifier.Prediction 

Structure

# MLHandActionClassifier.Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct Prediction
```

## Topics

### Inspecting a prediction

var results: [(label: String, confidence: Double)]

An array of prediction labels and their confidences for a hand action.

var frameRange: Range&lt;Int>

The range of frame rates the hand action classifier used to make its prediction.

## Relationships

### Conforms To

- Sendable

## See Also

### Testing a hand action classifier

func prediction(from: URL) throws -> [MLHandActionClassifier.Prediction]

Generates a hand action prediction for a video.

func predictions(from: [URL]) throws -> [[MLHandActionClassifier.Prediction]]

Generates an array of hand action predictions for each video in a URL array.

