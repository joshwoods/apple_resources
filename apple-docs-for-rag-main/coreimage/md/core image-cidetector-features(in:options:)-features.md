

- Core Image
- CIDetector
-  features(in:options:) 

Instance Method

# features(in:options:)

Searches for features in an image based on the specified image orientation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func features(
    in image: CIImage,
    options: [String : Any]? = nil
) -> [CIFeature]
```

## Parameters 

`image`  

The image you want to examine.

`options`  

A dictionary that specifies feature detection options. See Feature Detection Keys for allowed keys and their possible values.

## Return Value

An array of CIFeature objects. Each object represents a feature detected in the image.

## See Also

### Using a Detector Object to Find Features

func features(in: CIImage) -> [CIFeature]

Searches for features in an image.

