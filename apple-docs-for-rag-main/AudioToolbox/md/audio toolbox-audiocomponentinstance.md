

- Audio Toolbox
-  AudioComponentInstance 

Type Alias

# AudioComponentInstance

A component instance, or object, is an audio unit or audio codec.

iOSiPadOSMac CatalystmacOStvOSvisionOS

**macOS**

``` source
typealias AudioComponentInstance = UnsafeMutablePointer
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
typealias AudioComponentInstance = OpaquePointer
```

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

struct AudioComponentFlags

typealias AudioComponentFactoryFunction

