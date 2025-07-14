

- Core Video
-  CVFillExtendedPixelsCallBack 

Type Alias

# CVFillExtendedPixelsCallBack

Defines a pointer to a custom extended pixel-fill function, which is called whenever the system needs to pad a buffer holding your custom pixel format.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
typealias CVFillExtendedPixelsCallBack = (CVPixelBuffer, UnsafeMutableRawPointer?) -> DarwinBoolean
```

## Parameters 

`pixelBuffer`  

The pixel buffer to be padded.

`refCon`  

A pointer to application-defined data. This is the same value you stored in the CVFillExtendedPixelsCallBackData structure.

## Return Value

If `true`, the padding was successful; otherwise, `false`.

