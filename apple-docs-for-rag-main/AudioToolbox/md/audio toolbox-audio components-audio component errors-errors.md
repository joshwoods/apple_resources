

- Audio Toolbox
- Audio Components
-  Audio Component Errors 

API Collection

# Audio Component Errors

## Topics

### Constants

var kAudioComponentErr_DuplicateDescription: OSStatus

var kAudioComponentErr_InitializationTimedOut: OSStatus

var kAudioComponentErr_InvalidFormat: OSStatus

var kAudioComponentErr_NotPermitted: OSStatus

var kAudioComponentErr_TooManyInstances: OSStatus

var kAudioComponentErr_UnsupportedType: OSStatus

## See Also

### Creating an Audio Component Instance

func AudioComponentInstanceNew(AudioComponent, UnsafeMutablePointer&lt;AudioComponentInstance?>) -> OSStatus

Creates a new instance of an audio component.

func AudioComponentInstantiate(AudioComponent, AudioComponentInstantiationOptions, (AudioComponentInstance?, OSStatus) -> Void)

func AudioComponentInstanceDispose(AudioComponentInstance) -> OSStatus

Disposes of an audio component instance.

typealias AudioComponent

An audio component.

struct AudioComponentInstantiationOptions

