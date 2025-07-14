

- Core Image
- CIImage
- CIImageOption
-  nearestSampling 

Type Property

# nearestSampling

The key into the properties dictionary to indicate whether to use nearest-neighbor sampling.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let nearestSampling: CIImageOption
```

## Discussion

The value for this key is an NSNumber containing a Boolean value specifying whether the image should be sampled using nearest neighbor behavior. An unspecified value defaults to linear sampling.

