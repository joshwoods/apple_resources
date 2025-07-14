

- Create ML
- MLHandPoseClassifier
-  prediction(from:) 

Instance Method

# prediction(from:)

Generates a hand pose prediction for an image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func prediction(from image: URL) throws -> [(label: String, confidence: Double)]
```

## Return Value

An array of prediction tuples.

## Discussion

Each prediction consists of an array of tuples that pair a classification label with the model’s confidence in that label.

## See Also

### Testing a hand pose classifier

func predictions(from: [URL]) throws -> [[(label: String, confidence: Double)]]

Generates an array of hand pose predictions for each image in a URL array.

