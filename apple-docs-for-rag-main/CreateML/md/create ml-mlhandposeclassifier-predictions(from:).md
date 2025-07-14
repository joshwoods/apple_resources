

- Create ML
- MLHandPoseClassifier
-  predictions(from:) 

Instance Method

# predictions(from:)

Generates an array of hand pose predictions for each image in a URL array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func predictions(from images: [URL]) throws -> [[(label: String, confidence: Double)]]
```

## Parameters 

`images`  

An array of image file URLs.

## Return Value

An array of a prediction tuple arrays.

## Discussion

Each prediction consists of an array of tuples that pair a classification label with the model’s confidence for that label. The method returns an array of prediction arrays, where each element of the outer array is the prediction for the corresponding URL element in `images`.

## See Also

### Testing a hand pose classifier

func prediction(from: URL) throws -> [(label: String, confidence: Double)]

Generates a hand pose prediction for an image.

