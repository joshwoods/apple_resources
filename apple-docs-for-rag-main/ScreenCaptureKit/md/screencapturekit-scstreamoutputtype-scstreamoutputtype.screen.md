

- ScreenCaptureKit
- SCStreamOutputType
-  SCStreamOutputType.screen 

Case

# SCStreamOutputType.screen

An output type that represents a screen capture sample buffer.

Mac Catalyst 18.2+macOS 12.3+

``` source
case screen
```

## Discussion

This output represents a sample buffer that wraps a CVPixelBuffer backed by an IOSurface.

The width, height, and pixel format of the sample buffer reflect what you define in SCStreamConfiguration. When capturing multiple windows, the system bases the width and height on the display you pass in through SCContentFilter. You can set a background color for multi-window sample buffers by setting backgroundColor; otherwise the default color is black.

## See Also

### Output types

case audio

An output type that represents an audio capture sample buffer.

