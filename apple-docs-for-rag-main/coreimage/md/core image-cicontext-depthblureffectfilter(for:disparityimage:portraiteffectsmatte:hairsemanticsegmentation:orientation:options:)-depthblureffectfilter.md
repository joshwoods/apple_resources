

- Core Image
- CIContext
-  depthBlurEffectFilter(for:disparityImage:portraitEffectsMatte:hairSemanticSegmentation:orientation:options:) 

Instance Method

# depthBlurEffectFilter(for:disparityImage:portraitEffectsMatte:hairSemanticSegmentation:orientation:options:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func depthBlurEffectFilter(
    for image: CIImage,
    disparityImage: CIImage,
    portraitEffectsMatte: CIImage?,
    hairSemanticSegmentation: CIImage?,
    orientation: CGImagePropertyOrientation,
    options: [AnyHashable : Any]? = nil
) -> CIFilter?
```

## See Also

### Creating Depth Blur Filters

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, hairSemanticSegmentation: CIImage?, glassesMatte: CIImage?, gainMap: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(forImageData: Data, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(forImageURL: URL, options: [AnyHashable : Any]?) -> CIFilter?

