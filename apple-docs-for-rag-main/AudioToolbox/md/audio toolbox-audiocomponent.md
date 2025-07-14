

- Audio Toolbox
-  AudioComponent 

Type Alias

# AudioComponent

An audio component.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioComponent = OpaquePointer
```

## See Also

### Creating an Audio Component Instance

func AudioComponentInstanceNew(AudioComponent, UnsafeMutablePointer&lt;AudioComponentInstance?>) -> OSStatus

Creates a new instance of an audio component.

func AudioComponentInstantiate(AudioComponent, AudioComponentInstantiationOptions, (AudioComponentInstance?, OSStatus) -> Void)

func AudioComponentInstanceDispose(AudioComponentInstance) -> OSStatus

Disposes of an audio component instance.

struct AudioComponentInstantiationOptions

Audio Component Errors

