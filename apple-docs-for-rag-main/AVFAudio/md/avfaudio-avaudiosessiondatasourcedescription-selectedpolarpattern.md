

- AVFAudio
- AVAudioSessionDataSourceDescription
-  selectedPolarPattern 

Instance Property

# selectedPolarPattern

The data source’s active polar pattern.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var selectedPolarPattern: AVAudioSession.PolarPattern? { get }
```

## Discussion

If this value is nil, the data source doesn’t support directivity configuration.

## See Also

### Configuring Microphone Directivity

var supportedPolarPatterns: [AVAudioSession.PolarPattern]?

The set of directivity configurations supported by the data source.

var preferredPolarPattern: AVAudioSession.PolarPattern?

The preferred directivity configuration for the data source.

func setPreferredPolarPattern(AVAudioSession.PolarPattern?) throws

Selects the preferred directivity configuration for the data source.

struct PolarPattern

Constants that describe the possible polar patterns of the data source on an iOS device.

