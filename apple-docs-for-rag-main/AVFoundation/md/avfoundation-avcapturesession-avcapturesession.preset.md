

- AVFoundation
- AVCaptureSession
-  AVCaptureSession.Preset 

Structure

# AVCaptureSession.Preset

Presets that define standard configurations for a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
struct Preset
```

## Discussion

Setting a sessionPreset value provides a convenient way to configure a capture session for common use cases.

## Topics

### Quality Levels

static let high: AVCaptureSession.Preset

A preset suitable for capturing high-quality output.

static let medium: AVCaptureSession.Preset

A preset suitable for capturing medium-quality output.

static let low: AVCaptureSession.Preset

A preset suitable for capturing low-quality output.

### Photo

static let photo: AVCaptureSession.Preset

A preset suitable for capturing high-resolution photo quality output.

### Manual Configuration

static let inputPriority: AVCaptureSession.Preset

A preset that doesn’t specify audio and video output settings for a capture session.

### High Definition

static let qHD960x540: AVCaptureSession.Preset

A preset suitable for capturing quarter HD quality (960 x 540 pixel) video output.

static let hd1280x720: AVCaptureSession.Preset

A preset suitable for capturing 720p quality (1280 x 720 pixel) video output.

static let hd1920x1080: AVCaptureSession.Preset

A preset suitable for capturing 1080p-quality (1920 x 1080 pixels) video output.

static let hd4K3840x2160: AVCaptureSession.Preset

A preset suitable for capturing 2160p-quality (3840 x 2160 pixels) video output.

### VGA

static let qvga320x240: AVCaptureSession.Preset

A preset suitable for capturing 320 x 240 pixel video output.

static let vga640x480: AVCaptureSession.Preset

A preset suitable for capturing VGA quality (640 x 480 pixel) video output.

### iFrame

static let iFrame960x540: AVCaptureSession.Preset

A preset suitable for capturing 960 x 540 quality iFrame H.264 video at about 30 Mbits/sec with AAC audio.

static let iFrame1280x720: AVCaptureSession.Preset

A preset suitable for capturing 1280 x 720 quality iFrame H.264 video at about 40 Mbits/sec with AAC audio.

### CIF

static let cif352x288: AVCaptureSession.Preset

A preset suitable for capturing CIF quality (352 x 288 pixel) video output.

### Initializers

init(rawValue: String)

Creates a preset with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting a Session Preset

func canSetSessionPreset(AVCaptureSession.Preset) -> Bool

Determines whether you can configure a capture session with the specified preset.

var sessionPreset: AVCaptureSession.Preset

A preset value that indicates the quality level or bit rate of the output.

