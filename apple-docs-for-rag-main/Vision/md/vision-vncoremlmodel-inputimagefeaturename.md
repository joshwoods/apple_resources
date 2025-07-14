

- Vision
- VNCoreMLModel
-  inputImageFeatureName 

Instance Property

# inputImageFeatureName

The name of the feature value that Vision sets from the request handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var inputImageFeatureName: String { get set }
```

## Discussion

By default, Vision uses the first input found, but you can manually set that input to another featureName instead.

## See Also

### Providing Features

var featureProvider: (any MLFeatureProvider)?

An optional object to support inputs outside Vision.

