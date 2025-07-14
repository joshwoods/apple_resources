

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  AVCaptureDevice.Format.AutoFocusSystem 

Enumeration

# AVCaptureDevice.Format.AutoFocusSystem

An enumeration of auto focus systems.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
enum AutoFocusSystem
```

## Topics

### Systems

case none

Autofocus isn’t available.

case contrastDetection

A slower autofocus system based on differences in contrast.

case phaseDetection

A faster autofoscus system based on differences in light phase.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining the Auto Focus System

var autoFocusSystem: AVCaptureDevice.Format.AutoFocusSystem

The auto focus system the format uses.

