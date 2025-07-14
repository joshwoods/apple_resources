

- Audio Toolbox
-  AudioComponentDescription 

Structure

# AudioComponentDescription

Identifying information for an audio component.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioComponentDescription
```

## Topics

### Properties

var componentType: OSType

A unique 4-byte code identifying the interface for the component.

var componentSubType: OSType

A 4-byte code that you can use to indicate the purpose of a component. For example, you could use `lpas` or `lowp` as a mnemonic indication that an audio unit is a low-pass filter.

var componentManufacturer: OSType

The unique vendor identifier, registered with Apple, for the audio component.

var componentFlags: UInt32

Set this value to zero.

var componentFlagsMask: UInt32

Set this value to zero.

### Initializers

init()

init(componentType: OSType, componentSubType: OSType, componentManufacturer: OSType, componentFlags: UInt32, componentFlagsMask: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating an Audio Component Dynamically

func AudioComponentRegister(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioComponentFactoryFunction) -> AudioComponent

func AudioComponentCount(UnsafePointer&lt;AudioComponentDescription>) -> UInt32

Returns the number of audio components that match a specified `AudioComponentDescription` structure.

func AudioComponentFindNext(AudioComponent?, UnsafePointer&lt;AudioComponentDescription>) -> AudioComponent?

Finds the next component that matches a specified `AudioComponentDescription` structure after a specified audio component.

func AudioComponentInstanceGetComponent(AudioComponentInstance) -> AudioComponent

Retrieves a reference to an audio component from an instance of that audio component.

typealias AudioComponentInstance

A component instance, or object, is an audio unit or audio codec.

struct AudioComponentFlags

typealias AudioComponentFactoryFunction

