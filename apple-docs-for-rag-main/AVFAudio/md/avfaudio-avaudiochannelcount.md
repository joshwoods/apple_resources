

- AVFAudio
-  AVAudioChannelCount 

Type Alias

# AVAudioChannelCount

The number of audio channels.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVAudioChannelCount = UInt32
```

## See Also

### Getting Audio Channel Layout Properties

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var layout: UnsafePointer&lt;AudioChannelLayout>

The underlying audio channel layout.

var layoutTag: AudioChannelLayoutTag

The audio channel’s underlying layout tag.

func isEqual(Any) -> Bool

Indicates whether another audio channel layout is exactly equal to the current layout.

