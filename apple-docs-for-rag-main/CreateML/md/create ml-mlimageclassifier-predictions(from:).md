

- Create ML
- MLImageClassifier
-  predictions(from:) 

Instance Method

# predictions(from:)

Generates predictions for an array of images.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func predictions(from images: [URL]) throws -> [String]
```

## Parameters 

`images`  

An array of images you want the model to classify.

## Return Value

An array of prediction labels for the images. Each label’s index corresponds to the image’s index in the input array.

## See Also

### Testing an image classifier

func prediction(from: CGImage) throws -> String

Generates a prediction for an image.

func prediction(from: URL) throws -> String

Generates a prediction for an image at the URL.

