

- Audio Toolbox
-  ScheduledAudioSlice 

Structure

# ScheduledAudioSlice

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct ScheduledAudioSlice
```

## Topics

### Initializers

init(mTimeStamp: AudioTimeStamp, mCompletionProc: ScheduledAudioSliceCompletionProc?, mCompletionProcUserData: UnsafeMutableRawPointer, mFlags: AUScheduledAudioSliceFlags, mReserved: UInt32, mReserved2: UnsafeMutableRawPointer?, mNumberFrames: UInt32, mBufferList: UnsafeMutablePointer&lt;AudioBufferList>)

### Instance Properties

var mBufferList: UnsafeMutablePointer&lt;AudioBufferList>

var mCompletionProc: ScheduledAudioSliceCompletionProc?

var mCompletionProcUserData: UnsafeMutableRawPointer

var mFlags: AUScheduledAudioSliceFlags

var mNumberFrames: UInt32

var mReserved: UInt32

var mReserved2: UnsafeMutableRawPointer?

var mTimeStamp: AudioTimeStamp

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Audio Unit Types

struct ScheduledAudioFileRegion

typealias ScheduledAudioFileRegionCompletionProc

typealias ScheduledAudioSliceCompletionProc

typealias MIDIChannelNumber

MIDI Channel, 0~15 (channels 1 through 16, respectively).

typealias AUAudioObjectID

typealias AUMIDICIProfileChangedBlock

typealias AUAudioChannelCount

A number of audio channels.

typealias AUAudioFrameCount

A number of audio sample frames.

typealias AUAudioUnitStatus

A result code returned from an audio unit’s render function.

typealias AUEventListenerProc

typealias AUEventListenerRef

typealias AUEventSampleTime

Expresses time as a sample count.

typealias AUImplementorValueObserver

A block called to notify the audio unit implementation of changes to a parameter value.

typealias AUImplementorValueProvider

A block called to fetch a parameter’s current value from the audio unit implementation.

typealias AUInputHandler

A block to notify the host of an I/O unit that an input is available.

