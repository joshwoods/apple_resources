

- Audio Toolbox
-  kAudioQueueHardwareCodecPolicy_Default 

Global Variable

# kAudioQueueHardwareCodecPolicy_Default

If the required codec is available in both hardware and software implementations, the audio queue will use a hardware codec if its audio session category permits; it will use a software codec otherwise. If the required codec is available in only one form, that codec implementation is used.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
var kAudioQueueHardwareCodecPolicy_Default: UInt32 { get }
```

## See Also

### Constants

var kAudioQueueProperty_HardwareCodecPolicy: AudioQueuePropertyID

The preferred codec implementation type—hardware or software—for an audio queue. Possible values for this constant are the remaining constants described in this section.

var kAudioQueueHardwareCodecPolicy_UseSoftwareOnly: UInt32

The audio queue will use a software codec if one is available.

var kAudioQueueHardwareCodecPolicy_UseHardwareOnly: UInt32

The audio queue will use a hardware codec if one is available and if its use is permitted by the audio session category that you have set.

var kAudioQueueHardwareCodecPolicy_PreferSoftware: UInt32

The audio queue will use a software codec if one is available; if not, it will use a hardware codec if one is available and if its use is permitted by the audio session category that you have set.

var kAudioQueueHardwareCodecPolicy_PreferHardware: UInt32

The audio queue will use a hardware codec if one is available and if its use permitted by the audio session category that you have set; otherwise, it will use a software codec if one is available.

