

- Vision
- VNCoreMLModel
-  featureProvider 

Instance Property

# featureProvider

An optional object to support inputs outside Vision.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var featureProvider: (any MLFeatureProvider)? { get set }
```

## Discussion

This optional object conforms to the MLFeatureProvider protocol that the model uses to predict inputs that are not supplied by Vision. Vision provides the MLModel with the image for the inputImageFeatureName via the `VNRequestHandler`.

A feature provider is necessary for models that have more than one required input. Models with only one image input won’t use the feature provider.

## See Also

### Providing Features

var inputImageFeatureName: String

The name of the feature value that Vision sets from the request handler.

