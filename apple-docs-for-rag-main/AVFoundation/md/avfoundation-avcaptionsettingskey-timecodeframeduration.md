

- AVFoundation
- AVCaptionSettingsKey
-  timeCodeFrameDuration 

Type Property

# timeCodeFrameDuration

A key that identifies the frame duration that the system uses for the time code.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
static let timeCodeFrameDuration: AVCaptionSettingsKey
```

## Discussion

Some formats, such as TTML, use time code notation to indicate the timing of a caption. Use this key to specify the frame rate of the time code.

## See Also

### Keys

static let mediaType: AVCaptionSettingsKey

A key that identifies the output media type of a caption conversion operation.

static let mediaSubType: AVCaptionSettingsKey

A key that identifies the output media subtype of a caption conversion operation.

static let useDropFrameTimeCode: AVCaptionSettingsKey

A key that identifies whether the system uses drop frame time code.

