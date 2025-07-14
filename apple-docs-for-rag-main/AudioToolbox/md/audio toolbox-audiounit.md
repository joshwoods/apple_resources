

- Audio Toolbox
-  AudioUnit 

Type Alias

# AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioUnit = AudioComponentInstance
```

## Discussion

The various types of audio units are described in the Audio Unit Types enumeration. The subtypes of audio units provided by Apple are described in Converter Audio Unit Subtypes, Effect Audio Unit Subtypes, Mixer Audio Unit Subtypes, and Input/Output Audio Unit Subtypes.

## See Also

### Initializing the Audio Unit

func AudioUnitInitialize(AudioUnit) -> OSStatus

Initializes an audio unit

func AudioUnitUninitialize(AudioUnit) -> OSStatus

Uninitializes an audio unit.

func AudioUnitProcess(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioUnitProcessMultiple(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;UnsafePointer&lt;AudioBufferList>>, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AudioBufferList>>) -> OSStatus

func AudioUnitReset(AudioUnit, AudioUnitScope, AudioUnitElement) -> OSStatus

Resets an audio unit’s render state.

