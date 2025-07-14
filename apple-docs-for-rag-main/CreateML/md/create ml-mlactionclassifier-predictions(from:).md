

- Create ML
- MLActionClassifier
-  predictions(from:) 

Instance Method

# predictions(from:)

Generates a sequence of predictions for each video input.

macOS 11.0+

``` source
func predictions(from videos: [URL]) throws -> [[MLActionClassifier.Prediction]]
```

## Return Value

A array of prediction arrays. The index of each inner array corresponds to the video index in the input array.

## Discussion

- videos: An array of locations to videos you want the action classifier to analyze.

## See Also

### Testing an action classifier

func prediction(from: URL) throws -> [MLActionClassifier.Prediction]

Generates a prediction for each action the classifier recognizes in the video.

struct Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

