

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  supportedDepthDataFormats 

Instance Property

# supportedDepthDataFormats

The list of data formats compatible with this video format.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var supportedDepthDataFormats: [AVCaptureDevice.Format] { get }
```

## Discussion

Depth data capture requires a compatible pairing of video format and depth data format. After you set a capture device’s activeFormat property to this format, you can set the device’s activeDepthDataFormat property to one of the formats in this array.

Supported depth data formats always match the aspect ratio of their corresponding video format.

