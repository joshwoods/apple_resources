

- ARKit
- ARCamera
-  imageResolution 

Instance Property

# imageResolution

The width and height, in pixels, of the captured camera image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var imageResolution: CGSize { get }
```

## Discussion

This size describes the image in the capturedImage buffer, which contains image data in the camera device’s native sensor orientation. To convert image coordinates to match a specific display orientation of that image, use the viewMatrix(for:) or projectPoint(_:orientation:viewportSize:) method.

## See Also

### Examining Imaging Parameters

var intrinsics: simd_float3x3

A matrix that converts between the 2D camera plane and 3D world coordinate space.

