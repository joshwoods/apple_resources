

- Audio Toolbox
-  AudioComponentRegister(\_:\_:\_:\_:) 

Function

# AudioComponentRegister(\_:\_:\_:\_:)

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentRegister(
    _ inDesc: UnsafePointer,
    _ inName: CFString,
    _ inVersion: UInt32,
    _ inFactory: AudioComponentFactoryFunction
) -> AudioComponent
```

## See Also

### Creating an Audio Component Dynamically

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

struct AudioComponentFlags

typealias AudioComponentFactoryFunction

