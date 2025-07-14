

- AVFoundation
- AVAssetWriterInputPixelBufferAdaptor
-  append(\_:withPresentationTime:) 

Instance Method

# append(\_:withPresentationTime:)

Appends a pixel buffer to the adaptor.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func append(
    _ pixelBuffer: CVPixelBuffer,
    withPresentationTime presentationTime: CMTime
) -> Bool
```

## Parameters 

`pixelBuffer`  

The pixel buffer to append.

`presentationTime`  

The pixel buffer’s presentation time. The time you specify is relative to the time you called startSession(atSourceTime:) with.

## Return Value

true if the adaptor appends the pixel buffer; otherwise, false.

