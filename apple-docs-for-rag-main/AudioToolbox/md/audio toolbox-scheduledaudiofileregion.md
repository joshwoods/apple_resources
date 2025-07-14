

- Audio Toolbox
-  ScheduledAudioFileRegion 

Structure

# ScheduledAudioFileRegion

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct ScheduledAudioFileRegion
```

## Topics

### Initializers

init(mTimeStamp: AudioTimeStamp, mCompletionProc: ScheduledAudioFileRegionCompletionProc?, mCompletionProcUserData: UnsafeMutableRawPointer?, mAudioFile: OpaquePointer, mLoopCount: UInt32, mStartFrame: Int64, mFramesToPlay: UInt32)

### Instance Properties

var mAudioFile: OpaquePointer

Must be a valid and already-open audio file object (of type `AudioFileID`), as declared in `AudioToolbox/AudioFile.h`.

var mCompletionProc: ScheduledAudioFileRegionCompletionProc?

may be `NULL`

var mCompletionProcUserData: UnsafeMutableRawPointer?

var mFramesToPlay: UInt32

The number of frames to play.

var mLoopCount: UInt32

`0` = do not loop

var mStartFrame: Int64

The frame offset into the file.

var mTimeStamp: AudioTimeStamp

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Audio Unit Types

struct ScheduledAudioSlice

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

