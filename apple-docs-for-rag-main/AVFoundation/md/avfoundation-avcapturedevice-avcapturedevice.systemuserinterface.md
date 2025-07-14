

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.SystemUserInterface 

Enumeration

# AVCaptureDevice.SystemUserInterface

Constants that describe the capture device configuration user interfaces.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
enum SystemUserInterface
```

## Topics

### User Interfaces

case videoEffects

The system user interface for changing the state of video effects.

case microphoneModes

The system user interface for selecting microphone modes.

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

### Presenting the Configuration User Interface

class func showSystemUserInterface(AVCaptureDevice.SystemUserInterface)

Displays the system’s user interface to configure video effects or microphone modes.

