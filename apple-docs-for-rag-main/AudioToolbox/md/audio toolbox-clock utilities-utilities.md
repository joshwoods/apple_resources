

- Audio Toolbox
-  Clock Utilities 

API Collection

# Clock Utilities

Manage time-related information associated with audio playback.

## Topics

### Creating a Clock

func CAClockNew(UInt32, UnsafeMutablePointer&lt;CAClockRef?>) -> OSStatus

func CAClockDispose(CAClockRef) -> OSStatus

typealias CAClockRef

### Starting and Stopping the Clock

func CAClockStart(CAClockRef) -> OSStatus

func CAClockStop(CAClockRef) -> OSStatus

func CAClockArm(CAClockRef) -> OSStatus

func CAClockDisarm(CAClockRef) -> OSStatus

### Adding and Removing Listeners

func CAClockAddListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

func CAClockRemoveListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

typealias CAClockListenerProc

enum CAClockMessage

### Accessing the Current Time

func CAClockGetCurrentTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

func CAClockSetCurrentTime(CAClockRef, UnsafePointer&lt;CAClockTime>) -> OSStatus

func CAClockGetStartTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

struct CAClockTime

enum CAClockTimeFormat

typealias CAClockSamples

### Accessing Tempo Information

func CAClockGetCurrentTempo(CAClockRef, UnsafeMutablePointer&lt;CAClockTempo>, UnsafeMutablePointer&lt;CAClockTime>?) -> OSStatus

func CAClockSetCurrentTempo(CAClockRef, CAClockTempo, UnsafePointer&lt;CAClockTime>?) -> OSStatus

func CAClockGetPlayRate(CAClockRef, UnsafeMutablePointer&lt;Float64>) -> OSStatus

func CAClockSetPlayRate(CAClockRef, Float64) -> OSStatus

typealias CAClockTempo

struct CATempoMapEntry

### Accessing Clock Properties

func CAClockGetProperty(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func CAClockGetPropertyInfo(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

func CAClockSetProperty(CAClockRef, CAClockPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

enum CAClockPropertyID

enum CAClockSyncMode

### Parsing MIDI Data

func CAClockParseMIDI(CAClockRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

### Converting Time Values

func CAClockBarBeatTimeToBeats(CAClockRef, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;CAClockBeats>) -> OSStatus

func CAClockBeatsToBarBeatTime(CAClockRef, CAClockBeats, UInt16, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

func CAClockSMPTETimeToSeconds(CAClockRef, UnsafePointer&lt;SMPTETime>, UnsafeMutablePointer&lt;CAClockSeconds>) -> OSStatus

func CAClockSecondsToSMPTETime(CAClockRef, CAClockSeconds, UInt16, UnsafeMutablePointer&lt;SMPTETime>) -> OSStatus

func CAClockTranslateTime(CAClockRef, UnsafePointer&lt;CAClockTime>, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CABarBeatTime

struct CAMeterTrackEntry

### Getting Clock-Related Errors

Clock Errors

## See Also

### Utilities

Analyzing audio performance with Instruments

Ensure a smooth and immersive audio experience in your apps using Audio System Trace.

Audio Converter Services

Convert between linear PCM audio formats, and between linear PCM and compressed formats.

Audio Session Support

Describe the properties that you associate with audio sessions and audio routes.

Audio Toolbox Debugging

Obtain the internal state of Core Audio objects during the development and debugging of your code.

Workgroup Management

Coordinate the activity of custom real-time audio threads with those of the system and other processes.

Audio Codec

Translate audio data from one format to another.

