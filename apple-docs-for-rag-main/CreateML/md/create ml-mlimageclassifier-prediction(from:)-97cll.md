

- Create ML
- MLImageClassifier
-  prediction(from:) 

Instance Method

# prediction(from:)

Generates a prediction for an image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func prediction(from image: CGImage) throws -> String
```

## Parameters 

`image`  

The image that you want the model to classify.

## Return Value

A prediction label for the image.

## See Also

### Testing an image classifier

func prediction(from: URL) throws -> String

Generates a prediction for an image at the URL.

func predictions(from: [URL]) throws -> [String]

Generates predictions for an array of images.

