

- Vision
- VNImageOption
-  ciContext 

Type Property

# ciContext

An option key to specify the context to use in the handler’s Core Image operations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let ciContext: VNImageOption
```

## Discussion

If this key isn’t specified, Vision will create its own CIContext.

Specify a CIContext when you’ve used one in processing an input CIImage or executing a CIFilter chain, so you can save the cost of creating a new context.

## See Also

### Options Dictionary Keys

static let properties: VNImageOption

The dictionary from the image source that contains the metadata for algorithms like horizon detection.

static let cameraIntrinsics: VNImageOption

An option to specify the camera intrinstics.

