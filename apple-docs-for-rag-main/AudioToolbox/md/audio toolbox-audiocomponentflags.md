

- Audio Toolbox
-  AudioComponentFlags 

Structure

# AudioComponentFlags

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioComponentFlags
```

## Topics

### Flags

static var unsearchable: AudioComponentFlags

static var sandboxSafe: AudioComponentFlags

static var isV3AudioUnit: AudioComponentFlags

static var requiresAsyncInstantiation: AudioComponentFlags

static var canLoadInProcess: AudioComponentFlags

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating an Audio Component Dynamically

func AudioComponentRegister(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioComponentFactoryFunction) -> AudioComponent

func AudioComponentCount(UnsafePointer&lt;AudioComponentDescription>) -> UInt32

Returns the number of audio components that match a specified `AudioComponentDescription` structure.

func AudioComponentFindNext(AudioComponent?, UnsafePointer&lt;AudioComponentDescription>) -> AudioComponent?

Finds the next component that matches a specified `AudioComponentDescription` structure after a specified audio component.

func AudioComponentInstanceGetComponent(AudioComponentInstance) -> AudioComponent

Retrieves a reference to an audio component from an instance of that audio component.

struct AudioComponentDescription

Identifying information for an audio component.

typealias AudioComponentInstance

A component instance, or object, is an audio unit or audio codec.

typealias AudioComponentFactoryFunction

