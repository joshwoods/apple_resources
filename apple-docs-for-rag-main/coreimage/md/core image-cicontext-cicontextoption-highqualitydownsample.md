

- Core Image
- CIContext
- CIContextOption
-  highQualityDownsample 

Type Property

# highQualityDownsample

An option controlling the quality of image downsampling operations performed by the context.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static let highQualityDownsample: CIContextOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. A value of `true` (the default in macOS) results in higher image quality and lower performance. In iOS and tvOS, the default value is `false`.

