

- Core Audio
-  AudioHardwareSystem 

Class

# AudioHardwareSystem

macOS 15.0+

``` source
class AudioHardwareSystem
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var allowsHogMode: Bool

var allowsSleeping: Bool

var allowsUnloading: Bool

var boxes: [AudioHardwareBox]

var clocks: [AudioHardwareClock]

var defaultInputDevice: AudioHardwareDevice?

var defaultOutputDevice: AudioHardwareDevice?

var defaultSoundEffectsDevice: AudioHardwareDevice?

var devices: [AudioHardwareDevice]

var isInitializingOrExiting: Bool

var isProcessInputMuted: Bool

var plugins: [AudioHardwarePlugin]

var powerHint: AudioHardwarePowerHint

var processes: [AudioHardwareProcess]

var shouldMixStereoToMono: Bool

var taps: [AudioHardwareTap]

### Instance Methods

func box(forUID: String) throws -> AudioHardwareBox?

func clock(forUID: String) throws -> AudioHardwareClock?

func destroyAggregateDevice(AudioHardwareAggregateDevice) throws

func destroyProcessTap(AudioHardwareTap) throws

func device(forUID: String) throws -> AudioHardwareDevice?

func makeAggregateDevice(description: [String : Any]) throws -> AudioHardwareAggregateDevice?

func makeProcessTap(description: CATapDescription) throws -> AudioHardwareTap?

func plugin(forBundleID: String) throws -> AudioHardwarePlugin?

func process(for: pid_t) throws -> AudioHardwareProcess?

func setAllowsHogMode(Bool) throws

func setAllowsSleeping(Bool) throws

func setAllowsUnloading(Bool) throws

func setDefaultInputDevice(AudioHardwareDevice) throws

func setDefaultOutputDevice(AudioHardwareDevice) throws

func setDefaultSoundEffectsDevice(AudioHardwareDevice) throws

func setIsProcessInputMuted(Bool) throws

func setPowerHint(AudioHardwarePowerHint) throws

func setShouldMixStereoToMono(Bool) throws

func tap(forUID: String) throws -> AudioHardwareTap?

func unload() throws

### Type Properties

static let shared: AudioHardwareSystem

## Relationships

### Inherits From

- AudioHardwareObject

