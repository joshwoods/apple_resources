

- Audio Toolbox
-  kAudioQueueProperty_EnableLevelMetering 

Global Variable

# kAudioQueueProperty_EnableLevelMetering

Value is a read/write `UInt32` value that indicates whether audio level metering is enabled for an audio queue. `0` = metering off, `1` = metering on.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioQueueProperty_EnableLevelMetering: AudioQueuePropertyID { get }
```

## See Also

### Constants

var kAudioQueueDeviceProperty_NumberChannels: AudioQueuePropertyID

Value is a read-only `UInt32` value representing the number of channels in the audio hardware device associated with an audio queue.

var kAudioQueueDeviceProperty_SampleRate: AudioQueuePropertyID

Value is a read-only `Float64` value representing the sampling rate of the audio hardware device associated with an audio queue.

var kAudioQueueProperty_ChannelLayout: AudioQueuePropertyID

Describes an audio queue channel layout.

var kAudioQueueProperty_ConverterError: AudioQueuePropertyID

Value is a read-only `UInt32` value that indicates the most recent error (if any) encountered by the audio queue’s internal encoding/decoding process.

var kAudioQueueProperty_CurrentDevice: AudioQueuePropertyID

The unique identifier (UID) of the audio hardware device.

var kAudioQueueProperty_CurrentLevelMeter: AudioQueuePropertyID

A read-only array of level meter status structures.

var kAudioQueueProperty_CurrentLevelMeterDB: AudioQueuePropertyID

Value is a read-only array of AudioQueueLevelMeterState structures, one array element per audio channel. The member values in the structure are in decibels.

var kAudioQueueProperty_DecodeBufferSizeFrames: AudioQueuePropertyID

Value is a read/write `UInt32` value that is the size of the buffer into which a playback (output) audio queue decodes buffers. A larger buffer provides more reliability and better long-term performance at the expense of memory and decreased responsiveness in some situations.

var kAudioQueueProperty_EnableTimePitch: AudioQueuePropertyID

var kAudioQueueProperty_IsRunning: AudioQueuePropertyID

Value is a read-only `UInt32` value indicating whether or not the audio queue is running. A nonzero value means running; `0` means stopped. A notification is sent when the associated audio queue starts or stops, which may occur sometime after the AudioQueueStart(_:_:) or AudioQueueStop(_:_:) function is called.

var kAudioQueueProperty_MagicCookie: AudioQueuePropertyID

Value is a read/write void pointer to a block of memory, which you set up, containing an audio format magic cookie. If the audio format you are playing or recording to requires a magic cookie, you must set a value for this property before enqueuing any buffers.

var kAudioQueueProperty_MaximumOutputPacketSize: AudioQueuePropertyID

Value is a read-only`UInt32` value that is the size, in bytes, of the largest single packet of data in the output format. Primarily useful when encoding VBR compressed data.

var kAudioQueueProperty_StreamDescription: AudioQueuePropertyID

An audio queue’s data format.

var kAudioQueueProperty_TimePitchAlgorithm: AudioQueuePropertyID

var kAudioQueueProperty_TimePitchBypass: AudioQueuePropertyID

