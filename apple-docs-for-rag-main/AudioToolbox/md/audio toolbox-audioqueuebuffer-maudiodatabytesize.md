

- Audio Toolbox
- AudioQueueBuffer
-  mAudioDataByteSize 

Instance Property

# mAudioDataByteSize

The number of bytes of valid audio data in the audio queue buffer’s `mAudioData` field, initially set to `0`. Your callback must set this value for a playback audio queue; for recording, the recording audio queue sets the value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var mAudioDataByteSize: UInt32
```

