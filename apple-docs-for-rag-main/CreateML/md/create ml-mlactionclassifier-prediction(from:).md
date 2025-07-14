

- Create ML
- MLActionClassifier
-  prediction(from:) 

Instance Method

# prediction(from:)

Generates a prediction for each action the classifier recognizes in the video.

macOS 11.0+

``` source
func prediction(from video: URL) throws -> [MLActionClassifier.Prediction]
```

## Return Value

An array of predictions.

## Discussion

- video: The location of a video you want the action classifier to analyze.

## See Also

### Testing an action classifier

func predictions(from: [URL]) throws -> [[MLActionClassifier.Prediction]]

Generates a sequence of predictions for each video input.

struct Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

