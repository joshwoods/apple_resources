

- Core Image
- CIDetector
-  features(in:) 

Instance Method

# features(in:)

Searches for features in an image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func features(in image: CIImage) -> [CIFeature]
```

## Parameters 

`image`  

The image you want to examine.

## Return Value

An array of CIFeature objects. Each object represents a feature detected in the image.

## See Also

### Using a Detector Object to Find Features

func features(in: CIImage, options: [String : Any]?) -> [CIFeature]

Searches for features in an image based on the specified image orientation.

