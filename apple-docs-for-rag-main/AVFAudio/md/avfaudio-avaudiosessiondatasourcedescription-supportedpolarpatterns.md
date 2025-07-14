

- AVFAudio
- AVAudioSessionDataSourceDescription
-  supportedPolarPatterns 

Instance Property

# supportedPolarPatterns

The set of directivity configurations supported by the data source.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var supportedPolarPatterns: [AVAudioSession.PolarPattern]? { get }
```

## Discussion

This property returns an array of one or more polar patterns, or nil if the data source doesn’t support directivity configuration. This feature is available only on the built-in microphone port for certain devices.

## See Also

### Configuring Microphone Directivity

var selectedPolarPattern: AVAudioSession.PolarPattern?

The data source’s active polar pattern.

var preferredPolarPattern: AVAudioSession.PolarPattern?

The preferred directivity configuration for the data source.

func setPreferredPolarPattern(AVAudioSession.PolarPattern?) throws

Selects the preferred directivity configuration for the data source.

struct PolarPattern

Constants that describe the possible polar patterns of the data source on an iOS device.

