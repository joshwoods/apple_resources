

- Create ML
- MLActionClassifier
-  MLActionClassifier.Prediction 

Structure

# MLActionClassifier.Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

macOS 11.0+

``` source
struct Prediction
```

## Topics

### Inspecting a prediction

var results: [(label: String, confidence: Double)]

An array of prediction labels and their confidences for an action.

var frameRange: Range&lt;Int>

The range of frame rates the action classifier used to make its prediction.

## Relationships

### Conforms To

- Sendable

## See Also

### Testing an action classifier

func prediction(from: URL) throws -> [MLActionClassifier.Prediction]

Generates a prediction for each action the classifier recognizes in the video.

func predictions(from: [URL]) throws -> [[MLActionClassifier.Prediction]]

Generates a sequence of predictions for each video input.

