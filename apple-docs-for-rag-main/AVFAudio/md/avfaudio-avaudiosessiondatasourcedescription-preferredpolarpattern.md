

- AVFAudio
- AVAudioSessionDataSourceDescription
-  preferredPolarPattern 

Instance Property

# preferredPolarPattern

The preferred directivity configuration for the data source.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredPolarPattern: AVAudioSession.PolarPattern? { get }
```

## Discussion

If this value is nil, the data source doesn’t support directivity configuration, or you haven’t selected a preferred polar pattern.

## See Also

### Configuring Microphone Directivity

var selectedPolarPattern: AVAudioSession.PolarPattern?

The data source’s active polar pattern.

var supportedPolarPatterns: [AVAudioSession.PolarPattern]?

The set of directivity configurations supported by the data source.

func setPreferredPolarPattern(AVAudioSession.PolarPattern?) throws

Selects the preferred directivity configuration for the data source.

struct PolarPattern

Constants that describe the possible polar patterns of the data source on an iOS device.

