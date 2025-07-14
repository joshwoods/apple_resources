

- Core Image
- CIContext
-  depthBlurEffectFilter(for:disparityImage:portraitEffectsMatte:orientation:options:) 

Instance Method

# depthBlurEffectFilter(for:disparityImage:portraitEffectsMatte:orientation:options:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func depthBlurEffectFilter(
    for image: CIImage,
    disparityImage: CIImage,
    portraitEffectsMatte: CIImage?,
    orientation: CGImagePropertyOrientation,
    options: [AnyHashable : Any]? = nil
) -> CIFilter?
```

## See Also

### Creating Depth Blur Filters

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, hairSemanticSegmentation: CIImage?, glassesMatte: CIImage?, gainMap: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, hairSemanticSegmentation: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(forImageData: Data, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(forImageURL: URL, options: [AnyHashable : Any]?) -> CIFilter?

