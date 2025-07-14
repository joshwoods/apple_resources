

- AVFAudio
- AVAudioSessionDataSourceDescription
-  setPreferredPolarPattern(\_:) 

Instance Method

# setPreferredPolarPattern(\_:)

Selects the preferred directivity configuration for the data source.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setPreferredPolarPattern(_ pattern: AVAudioSession.PolarPattern?) throws
```

## Parameters 

`pattern`  

The directivity configuration to use.

## Discussion

Calling this method requests a change to the selected polar pattern. To determine whether the change has taken effect, inspect the selectedPolarPattern property.

If the data source and its owning port are in use, using this method to change the directivity configuration is likely to result in a route reconfiguration.

Set a preferred polar pattern only after setting the audio session’s category and mode, and activating the session.

## See Also

### Configuring Microphone Directivity

var selectedPolarPattern: AVAudioSession.PolarPattern?

The data source’s active polar pattern.

var supportedPolarPatterns: [AVAudioSession.PolarPattern]?

The set of directivity configurations supported by the data source.

var preferredPolarPattern: AVAudioSession.PolarPattern?

The preferred directivity configuration for the data source.

struct PolarPattern

Constants that describe the possible polar patterns of the data source on an iOS device.

