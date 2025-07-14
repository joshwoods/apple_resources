

- Audio Toolbox
-  AudioComponentInstantiationOptions 

Structure

# AudioComponentInstantiationOptions

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioComponentInstantiationOptions
```

## Topics

### Constants

static var loadInProcess: AudioComponentInstantiationOptions

static var loadOutOfProcess: AudioComponentInstantiationOptions

### Initializers

init(rawValue: UInt32)

### Type Properties

static var loadedRemotely: AudioComponentInstantiationOptions

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

### Creating an Audio Component Instance

func AudioComponentInstanceNew(AudioComponent, UnsafeMutablePointer&lt;AudioComponentInstance?>) -> OSStatus

Creates a new instance of an audio component.

func AudioComponentInstantiate(AudioComponent, AudioComponentInstantiationOptions, (AudioComponentInstance?, OSStatus) -> Void)

func AudioComponentInstanceDispose(AudioComponentInstance) -> OSStatus

Disposes of an audio component instance.

typealias AudioComponent

An audio component.

Audio Component Errors

