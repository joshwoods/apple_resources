

- Accelerate
- vImage
- vImage Operations
- Applying projective transformations to images
-  Transforming an image in three dimensions 

Article

# Transforming an image in three dimensions

Create and use a projective transformation to apply a perspective warp to an image.

## Overview

The vImage library provides a set of functions that allow you create projective-transformation structures and apply them to images. The following image shows the effect of a projective transformation that derives from the four corner points of a perspective distorted rectangle. The image demonstrates how the projective transformation warps the image to match the empty billboard rectangle.

### Create the vImage buffers that represent the source images

Create a vImage_CGImageFormat structure that describes the four-channel, 8-bit-per-channel images that this example uses.

```
var format = vImage_CGImageFormat(
    bitsPerComponent: 8,
    bitsPerPixel: 8 * 4,
    colorSpace: CGColorSpaceCreateDeviceRGB(),
    bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.noneSkipFirst.rawValue))!
```

Use separate buffers to store the background and foreground images.

```
let backgroundImage =  imageLiteral(resourceName: "background.jpg").cgImage(
    forProposedRect: nil,
    context: nil,
    hints: nil)!
let backgroundBuffer = try vImage.PixelBuffer(
    cgImage: backgroundImage,
    cgImageFormat: &format)

let foregroundImage =  imageLiteral(resourceName: "foreground.jpg").cgImage(
    forProposedRect: nil,
    context: nil,
    hints: nil)!
let foregroundBuffer = try vImage.PixelBuffer(
    cgImage: foregroundImage,
    cgImageFormat: &format)

```

Because the perspective warp doesn’t work in place (that is, the source and destination buffers must point to different underlying memory), create a third destination buffer.

```
let warpedBuffer = vImage.PixelBuffer(
    size: backgroundBuffer.size)
```

### Use the Vision framework to find the rectangle corner points

The Vision framework allows you to find the corner points of the target rectangle. The code below is a simplified example. See Detecting Objects in Still Images for additional information.

```
let imageRequestHandler = VNImageRequestHandler(cgImage: backgroundImage,
                                                options: [:])

let requests: [VNRequest] = [VNDetectRectanglesRequest()]

try imageRequestHandler.perform(requests)

guard let observation = requests.first?.results?.first as? VNRectangleObservation  else {
    throw vImage.Error.internalError
}
```

On return, `observation` contains the four corner points of the target rectangle.

### Create the source and destination points

Use the values in the Vision VNRectangleObservation instance to create a set of points for the vImage warp function. The Vision framework returns normalized coordinates in the range `0...1` with `0` at the bottom-left of the image. The vImage warp function requires coordinates that represent pixel values with `0` at the top-left of the image.

The destination points refer to the corner points of the target rectangle.

```
typealias vImagePoint = (Float, Float)

let dstPoints: [vImagePoint] = {
    func scalePoint(_ point: CGPoint) -> vImagePoint {
        return (Float(point.x) * Float(backgroundImage.width),
                Float(point.y) * Float(backgroundImage.height))
    }

    let dstTopLeft: vImagePoint = scalePoint(observation.topLeft)
    let dstTopRight: vImagePoint = scalePoint(observation.topRight)
    let dstBottomLeft: vImagePoint = scalePoint(observation.bottomLeft)
    let dstBottomRight: vImagePoint = scalePoint(observation.bottomRight)

    return [dstTopLeft, dstTopRight, dstBottomLeft, dstBottomRight]
}()

```

The source points refer to the bounding box of the foreground image.

```
let srcPoints: [vImagePoint] = {
    let foregroundWidth = Float(foregroundImage.width)
    let foregroundHeight = Float(foregroundImage.height)

    let srcTopLeft: (Float, Float) = (0, foregroundHeight)
    let srcTopRight: (Float, Float) = (foregroundWidth, foregroundHeight)
    let srcBottomLeft: (Float, Float) = (0, 0)
    let srcBottomRight: (Float, Float) = (foregroundWidth, 0)

    return [srcTopLeft, srcTopRight, srcBottomLeft, srcBottomRight]
}()

```

### Calculate the projective transformation

Call vImageGetPerspectiveWarp(_:_:_:_:) to calculate the projective transformation to translate the foreground image to the target rectangle.

```
var transform = vImage_PerpsectiveTransform()
vImageGetPerspectiveWarp(srcPoints, dstPoints, &transform, 0)

```

On return, `transform` contains the projective transformation to warp the source points to the destination points.

### Apply the perspective warp

Call vImagePerspectiveWarp_ARGB8888(_:_:_:_:_:_:_:) to warp the foreground image to the destination rectangle’s shape and position.

```
foregroundBuffer.withUnsafePointerToVImageBuffer { src in
    warpedBuffer.withUnsafePointerToVImageBuffer { dst in

        var bgColor: [UInt8] = [0, 0, 0, 0]

        vImagePerspectiveWarp_ARGB8888(
            src, dst, nil,
            &transform,
            vImage_WarpInterpolation(kvImageInterpolationLinear),
            &bgColor,
            vImage_Flags(kvImageBackgroundColorFill))
    }
}

```

### Composite the warped foreground over the background image

Finally, composite the warped foreground image over the background image.

```
backgroundBuffer.alphaComposite(.nonpremultiplied,
                                topLayer: warpedBuffer,
                                destination: backgroundBuffer)

let result = backgroundBuffer.makeCGImage(cgImageFormat: format)

```

## See Also

### Computing a projective transformation from source and destination quadrilaterals

func vImageGetPerspectiveWarp(UnsafePointer&lt;(Float, Float)>, UnsafePointer&lt;(Float, Float)>, UnsafeMutablePointer&lt;vImage_PerpsectiveTransform>, vImage_Flags) -> vImage_Error

Returns a projective-transformation structure that defines the mapping between a source quadrilateral and a destination quadrilateral.

struct vImage_PerpsectiveTransform

A projective-transformation matrix.

