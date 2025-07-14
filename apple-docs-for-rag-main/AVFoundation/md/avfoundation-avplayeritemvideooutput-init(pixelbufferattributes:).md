

- AVFoundation
- AVPlayerItemVideoOutput
-  init(pixelBufferAttributes:) 

Initializer

# init(pixelBufferAttributes:)

Creates a video output object using the specified pixel buffer attributes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
init(pixelBufferAttributes: [String : Any]? = nil)
```

## Parameters 

`pixelBufferAttributes`  

The pixel buffer attributes required for video output. For a list of pixel buffer attributes you can include in this dictionary, see the `CVPixelBuffer.h` header file in the Core Video framework.

## Return Value

An initialized video output object.

## See Also

### Creating a Video Output

init(outputSettings: [String : Any]?)

Creates a video output object initialized with the specified output settings.

