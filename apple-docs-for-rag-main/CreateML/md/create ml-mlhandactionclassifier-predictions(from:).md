

- Create ML
- MLHandActionClassifier
-  predictions(from:) 

Instance Method

# predictions(from:)

Generates an array of hand action predictions for each video in a URL array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func predictions(from videos: [URL]) throws -> [[MLHandActionClassifier.Prediction]]
```

## Parameters 

`videos`  

An array of video file URLs.

## Return Value

A array of prediction arrays. The index of each inner array corresponds to the video URL index in the input array.

## See Also

### Testing a hand action classifier

func prediction(from: URL) throws -> [MLHandActionClassifier.Prediction]

Generates a hand action prediction for a video.

struct Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

