

- Audio Toolbox
-  kAudioQueueProperty_HardwareCodecPolicy 

Global Variable

# kAudioQueueProperty_HardwareCodecPolicy

The preferred codec implementation type—hardware or software—for an audio queue. Possible values for this constant are the remaining constants described in this section.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
var kAudioQueueProperty_HardwareCodecPolicy: AudioQueuePropertyID { get }
```

## See Also

### Constants

var kAudioQueueHardwareCodecPolicy_Default: UInt32

If the required codec is available in both hardware and software implementations, the audio queue will use a hardware codec if its audio session category permits; it will use a software codec otherwise. If the required codec is available in only one form, that codec implementation is used.

var kAudioQueueHardwareCodecPolicy_UseSoftwareOnly: UInt32

The audio queue will use a software codec if one is available.

var kAudioQueueHardwareCodecPolicy_UseHardwareOnly: UInt32

The audio queue will use a hardware codec if one is available and if its use is permitted by the audio session category that you have set.

var kAudioQueueHardwareCodecPolicy_PreferSoftware: UInt32

The audio queue will use a software codec if one is available; if not, it will use a hardware codec if one is available and if its use is permitted by the audio session category that you have set.

var kAudioQueueHardwareCodecPolicy_PreferHardware: UInt32

The audio queue will use a hardware codec if one is available and if its use permitted by the audio session category that you have set; otherwise, it will use a software codec if one is available.

