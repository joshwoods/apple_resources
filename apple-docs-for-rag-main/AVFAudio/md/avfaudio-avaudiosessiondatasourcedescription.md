

- AVFAudio
-  AVAudioSessionDataSourceDescription 

Class

# AVAudioSessionDataSourceDescription

An object that defines a data source for an audio input or output, giving information such as the source’s name, location, and orientation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioSessionDataSourceDescription
```

## Overview

You obtain data source descriptions from the shared AVAudioSession object or the AVAudioSessionPortDescription objects corresponding to its input and output ports. Only built-in microphone ports on certain devices support the location, orientation, and polar pattern properties. If a port doesn’t support these features, the value of its dataSources property is `nil`.

This class is especially useful for differentiating between microphone configurations on devices having more than one built-in microphone. Such devices may also support signal processing features for spatial filtering, or *beamforming*, in which the system makes the device more sensitive to audio signals from a particular direction. See `Data Source Polar Patterns` for more information.

## Topics

### Identifying a Data Source

var dataSourceID: NSNumber

The system-assigned identifier for the data source.

var dataSourceName: String

A human-readable name for the data source.

### Retrieving the Data Source Location

var location: AVAudioSession.Location?

The location of the data source on the device.

struct Location

Constants that describe the location of the data source on device.

### Retrieving the Data Source Orientation

var orientation: AVAudioSession.Orientation?

The orientation of the data source relative to the device’s natural orientation.

struct Orientation

Constants that indicate the directions in which a data source can point, relative to the device’s natural orientation.

### Configuring Microphone Directivity

var selectedPolarPattern: AVAudioSession.PolarPattern?

The data source’s active polar pattern.

var supportedPolarPatterns: [AVAudioSession.PolarPattern]?

The set of directivity configurations supported by the data source.

var preferredPolarPattern: AVAudioSession.PolarPattern?

The preferred directivity configuration for the data source.

func setPreferredPolarPattern(AVAudioSession.PolarPattern?) throws

Selects the preferred directivity configuration for the data source.

struct PolarPattern

Constants that describe the possible polar patterns of the data source on an iOS device.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Configuring outputs

var outputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available output data sources for the current audio route.

var outputDataSource: AVAudioSessionDataSourceDescription?

The currently selected output data source.

func setOutputDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the output data source for an audio session.

func overrideOutputAudioPort(AVAudioSession.PortOverride) throws

Temporarily changes the current audio route.

