

- Core Video
-  CVPixelBufferReleasePlanarBytesCallback 

Type Alias

# CVPixelBufferReleasePlanarBytesCallback

Defines a pointer to a pixel buffer release callback function, which is called when a pixel buffer created by CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) is released.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
typealias CVPixelBufferReleasePlanarBytesCallback = (UnsafeMutableRawPointer?, UnsafeRawPointer?, Int, Int, UnsafeMutablePointer?) -> Void
```

## Parameters 

`releaseRefCon`  

A pointer to application-defined data. This pointer is the same as that passed in the `releaseRefCon` parameter of CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:).

`dataPtr`  

A pointer to a plane descriptor block. This is the same pointer you passed to CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) in the `dataPtr` parameter.

`dataSize`  

The size value you passed to CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) in the `dataSize` parameter.

`numberOfPlanes`  

The number of planes value you passed to CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) in the `numberOfPlanes` parameter.

`planeAddresses`  

A pointer to the base plane address you passed to CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) in the `basePlaneAddress` parameter.

## Discussion

You would declare a callback named `MyPixelBufferReleasePlanarBytes` like this:

### Discussion

You use this callback to release the pixels and perform any other cleanup when a pixel buffer is released.

## See Also

### Callbacks

typealias CVPixelBufferReleaseBytesCallback

A type that defines a release callback function.

