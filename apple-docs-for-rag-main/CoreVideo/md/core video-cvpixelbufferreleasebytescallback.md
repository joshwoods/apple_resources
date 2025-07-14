

- Core Video
-  CVPixelBufferReleaseBytesCallback 

Type Alias

# CVPixelBufferReleaseBytesCallback

A type that defines a release callback function.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
typealias CVPixelBufferReleaseBytesCallback = (UnsafeMutableRawPointer?, UnsafeRawPointer?) -> Void
```

## Parameters 

`releaseRefCon`  

A pointer to application-defined data. This pointer is the same as that passed in the `releaseRefCon` parameter of CVPixelBufferCreateWithBytes(_:_:_:_:_:_:_:_:_:_:).

`baseAddress`  

A pointer to the base address of the memory holding the pixels. This pointer is the same as that passed in the `baseAddress` parameter of CVPixelBufferCreateWithBytes(_:_:_:_:_:_:_:_:_:_:).

## Discussion

When you create a pixel buffer using CVPixelBufferCreateWithBytes(_:_:_:_:_:_:_:_:_:_:), you can optionally pass a callback function that’s invoked when the system frees the pixel buffer. Use this callback function to release the pixel data and perform any other cleanup needed when the buffer is released.

You define a callback function as shown below:

- Swift
- Objective-C

```
```

```
// Define a function to call when the pixel buffer is freed.
void releaseCallback(void *releaseRefCon, const void *baseAddress) {
    free((void *)baseAddress);
    // Perform additional cleanup as needed.
}
```

## See Also

### Callbacks

typealias CVPixelBufferReleasePlanarBytesCallback

Defines a pointer to a pixel buffer release callback function, which is called when a pixel buffer created by CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) is released.

