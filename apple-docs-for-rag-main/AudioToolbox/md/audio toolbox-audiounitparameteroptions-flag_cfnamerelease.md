

- Audio Toolbox
- AudioUnitParameterOptions
-  flag_CFNameRelease 

Type Property

# flag_CFNameRelease

If an audio unit can generate parameter names dynamically, it should set this flag.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var flag_CFNameRelease: AudioUnitParameterOptions { get }
```

## Discussion

Audio unit hosting applications should check for this flag being set. If it is, the host should release the audio unit parameter name when it is done using it.

If this flag is not set, the host application can assume that the audio unit will release its parameter names.

## See Also

### Constants

static var flag_CanRamp: AudioUnitParameterOptions

static var flag_DisplayCubeRoot: AudioUnitParameterOptions

static var flag_DisplayCubed: AudioUnitParameterOptions

static var flag_DisplayExponential: AudioUnitParameterOptions

static var flag_DisplayLogarithmic: AudioUnitParameterOptions

static var flag_DisplayMask: AudioUnitParameterOptions

static var flag_DisplaySquareRoot: AudioUnitParameterOptions

static var flag_DisplaySquared: AudioUnitParameterOptions

static var flag_ExpertMode: AudioUnitParameterOptions

static var flag_HasCFNameString: AudioUnitParameterOptions

static var flag_HasClump: AudioUnitParameterOptions

static var flag_IsElementMeta: AudioUnitParameterOptions

static var flag_IsGlobalMeta: AudioUnitParameterOptions

static var flag_IsHighResolution: AudioUnitParameterOptions

static var flag_IsReadable: AudioUnitParameterOptions

