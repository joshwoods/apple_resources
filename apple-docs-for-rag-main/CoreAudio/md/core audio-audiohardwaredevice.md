

- Core Audio
-  AudioHardwareDevice 

Class

# AudioHardwareDevice

macOS 15.0+

``` source
class AudioHardwareDevice
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var actualSampleRate: Double

var bufferFrameSize: Int

var bufferFrameSizeRange: AudioValueRange

var canBeDefaultInputDevice: Bool

var canBeDefaultOutputDevice: Bool

var canBeDefaultSoundEffectsDevice: Bool

var clock: AudioHardwareClock

var configurationApplication: String

var currentTime: AudioTimeStamp

var hogModePID: pid_t

var icon: URL?

var inputSafetyOffset: Int

var inputStreamConfiguration: [AudioBuffer]

var ioCycleUsage: Float

var isHidden: Bool

var isProcessInputMuted: Bool

var isProcessOutputMuted: Bool

var isRunningInAProcess: Bool

var largestVariableBufferFrameSize: Int

var modelUID: String

var outputSafetyOffset: Int

var outputStreamConfiguration: [AudioBuffer]

var preferredInputChannelsForStereo: [UInt32]

var preferredOutputChannelsForStereo: [UInt32]

var relatedDevices: [AudioHardwareDevice]

var streams: [AudioHardwareStream]

var usesVariableBufferFrameSizes: Bool

var workgroup: WorkGroup

### Instance Methods

func nearestStartTime(atTime: AudioTimeStamp, withFlags: UInt32) throws -> AudioTimeStamp

func setBufferFrameSize(Int) throws

func setClock(AudioHardwareClock) throws

func setIOCycleUsage(Float) throws

func setIsProcessInputMuted(Bool) throws

func setIsProcessOutputMuted(Bool) throws

func setPreferredInputChannelsForStereo([UInt32]) throws

func setPreferredOutputChannelsForStereo([UInt32]) throws

func start(IOProcID: AudioDeviceIOProcID?) throws

func start(at: AudioTimeStamp, flags: UInt32, IOProcID: AudioDeviceIOProcID?) throws -> AudioTimeStamp?

func stop(IOProcID: AudioDeviceIOProcID?) throws

func toggleHogMode() throws -> pid_t

func translateTime(AudioTimeStamp) throws -> AudioTimeStamp

## Relationships

### Inherits From

- AudioHardwareClock

### Inherited By

- AudioHardwareAggregateDevice

