

- AVFAudio
- AVAudioSession
-  AVAudioSession.Location 

Structure

# AVAudioSession.Location

Constants that describe the location of the data source on device.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct Location
```

## Topics

### Creating a Location

init(rawValue: String)

Creates a new instance with the raw value you specify.

### Getting Standard Locations

static let lower: AVAudioSession.Location

A value that indicates that the data source is located near the bottom end of the device.

static let upper: AVAudioSession.Location

A value that indicates that the data source is located near the top end of the device.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

### Type Properties

static var orientationBack: AVAudioSession.Location

static var orientationBottom: AVAudioSession.Location

static var orientationFront: AVAudioSession.Location

static var orientationLeft: AVAudioSession.Location

static var orientationRight: AVAudioSession.Location

static var orientationTop: AVAudioSession.Location

static var polarPatternCardioid: AVAudioSession.Location

static var polarPatternOmnidirectional: AVAudioSession.Location

static var polarPatternSubcardioid: AVAudioSession.Location

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving the Data Source Location

var location: AVAudioSession.Location?

The location of the data source on the device.

