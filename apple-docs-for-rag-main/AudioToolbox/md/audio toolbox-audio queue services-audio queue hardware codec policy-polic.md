

- Audio Toolbox
- Audio Queue Services
-  Audio Queue Hardware Codec Policy 

API Collection

# Audio Queue Hardware Codec Policy

## Topics

### Constants

var kAudioQueueHardwareCodecPolicy_Default: UInt32

If the required codec is available in both hardware and software implementations, the audio queue will use a hardware codec if its audio session category permits; it will use a software codec otherwise. If the required codec is available in only one form, that codec implementation is used.

var kAudioQueueHardwareCodecPolicy_PreferHardware: UInt32

The audio queue will use a hardware codec if one is available and if its use permitted by the audio session category that you have set; otherwise, it will use a software codec if one is available.

var kAudioQueueHardwareCodecPolicy_PreferSoftware: UInt32

The audio queue will use a software codec if one is available; if not, it will use a hardware codec if one is available and if its use is permitted by the audio session category that you have set.

var kAudioQueueHardwareCodecPolicy_UseHardwareOnly: UInt32

The audio queue will use a hardware codec if one is available and if its use is permitted by the audio session category that you have set.

var kAudioQueueHardwareCodecPolicy_UseSoftwareOnly: UInt32

The audio queue will use a software codec if one is available.

## See Also

### Enumerations

struct AudioQueueProcessingTapFlags

Anonymous

Audio Queue Time Pitch Algorithms

Audio Queue Property IDs

Audio Queue Property IDs

