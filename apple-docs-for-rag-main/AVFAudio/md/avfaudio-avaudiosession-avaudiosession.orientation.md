

- AVFAudio
- AVAudioSession
-  AVAudioSession.Orientation 

Structure

# AVAudioSession.Orientation

Constants that indicate the directions in which a data source can point, relative to the device’s natural orientation.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct Orientation
```

## Topics

### Creating an Orientation

init(rawValue: String)

Creates a new instance with the raw value you specify.

### Getting Standard Orientations

static let top: AVAudioSession.Orientation

A data source that points upward.

static let bottom: AVAudioSession.Orientation

A data source that points downward.

static let front: AVAudioSession.Orientation

A data source that points outward from the front of the device, toward the user.

static let back: AVAudioSession.Orientation

A data source that points outward from the back of the device, away from the user.

static let left: AVAudioSession.Orientation

A data source that points outward to the left of the device, away from the user.

static let right: AVAudioSession.Orientation

A data source that points outward to the right of the device, away from the user.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving the Data Source Orientation

var orientation: AVAudioSession.Orientation?

The orientation of the data source relative to the device’s natural orientation.

