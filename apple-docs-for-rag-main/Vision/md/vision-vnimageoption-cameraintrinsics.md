

- Vision
- VNImageOption
-  cameraIntrinsics 

Type Property

# cameraIntrinsics

An option to specify the camera intrinstics.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let cameraIntrinsics: VNImageOption
```

## Discussion

The camera intrinsics matrix is a CFData instance containing a matrix_float3x3, which is a column-major matrix:

`fx` and `fy` are the focal length in pixels. For square pixels, they have the same value.

`ox` and `oy` are the coordinates of the principal point. The origin is the upper-left corner of the frame.

## See Also

### Options Dictionary Keys

static let properties: VNImageOption

The dictionary from the image source that contains the metadata for algorithms like horizon detection.

static let ciContext: VNImageOption

An option key to specify the context to use in the handler’s Core Image operations.

