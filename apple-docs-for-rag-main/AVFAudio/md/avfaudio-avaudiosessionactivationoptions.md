

- AVFAudio
-  AVAudioSessionActivationOptions 

Structure

# AVAudioSessionActivationOptions

Constants that describe the options to pass when activating the audio session.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudioSessionActivationOptions
```

## Topics

### Getting Standard Activation Options

init(rawValue: UInt)

Creates a new instance with the raw value you specify.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Activating the audio configuration

func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws

Activates or deactivates your app’s audio session using the specified options.

func activate(options: AVAudioSessionActivationOptions, completionHandler: (Bool, (any Error)?) -> Void)

Activates an audio session asynchronously on watchOS.

