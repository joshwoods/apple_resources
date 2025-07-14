

- AVFAudio
-  AVAudioUnitDistortionPreset 

Enumeration

# AVAudioUnitDistortionPreset

Constants that represent preset audio distortions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVAudioUnitDistortionPreset
```

## Topics

### Presets

case drumsBitBrush

A preset that represents a bit brush drums distortion.

case drumsBufferBeats

A preset that represents a buffer beat drums distortion.

case drumsLoFi

A preset that represents a low fidelity drums distortion.

case multiBrokenSpeaker

A preset that represents a broken speaker distortion.

case multiCellphoneConcert

A preset that represents a cellphone concert distortion.

case multiDecimated1

A preset that represents a variant of the decimated distortion.

case multiDecimated2

A preset that represents a variant of the decimated distortion.

case multiDecimated3

A preset that represents a variant of the decimated distortion.

case multiDecimated4

A preset that represents a variant of the decimated distortion.

case multiDistortedFunk

A preset that represents a distorted funk distortion.

case multiDistortedCubed

A preset that represents a distorted cubed distortion.

case multiDistortedSquared

A preset that represents a distorted squared distortion.

case multiEcho1

A preset that represents a variant of an echo distortion.

case multiEcho2

A preset that represents a variant of an echo distortion.

case multiEchoTight1

A preset that represents a variant of a tight echo distortion.

case multiEchoTight2

A preset that represents a variant of a tight echo distortion.

case multiEverythingIsBroken

A preset that represents an everything-is-broken distortion.

case speechAlienChatter

A preset that represents an alien chatter distortion.

case speechCosmicInterference

A preset that represents a cosmic interference distortion.

case speechGoldenPi

A preset that represents a golden pi distortion.

case speechRadioTower

A preset that represents a radio tower distortion.

case speechWaves

A preset that represents a speech wave distortion.

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

### Configuring the distortion

func loadFactoryPreset(AVAudioUnitDistortionPreset)

Configures the audio distortion unit by loading a distortion preset.

