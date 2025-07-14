

- AVFoundation
- AVPlayerItemVideoOutput
-  init(outputSettings:) 

Initializer

# init(outputSettings:)

Creates a video output object initialized with the specified output settings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(outputSettings: [String : Any]?)
```

## Parameters 

`outputSettings`  

The client requirements for output CVPixelBuffer objects, expressed using the constants in `AVVideoSettings.h`.

## Discussion

For uncompressed video output, start with `kCVPixelBuffer*` keys in ``. In addition to the keys in `CVPixelBuffer.h`, uncompressed video settings dictionaries may also provide a value for AVVideoAllowWideColorKey.

## See Also

### Creating a Video Output

init(pixelBufferAttributes: [String : Any]?)

Creates a video output object using the specified pixel buffer attributes.

