

- Audio Toolbox
-  AudioComponentCount(\_:) 

Function

# AudioComponentCount(\_:)

Returns the number of audio components that match a specified `AudioComponentDescription` structure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentCount(_ inDesc: UnsafePointer) -> UInt32
```

## Parameters 

`inDesc`  

The description of the audio components you want to count.

## Return Value

The number of matching components on the system.

## See Also

### Creating an Audio Component Dynamically

func AudioComponentRegister(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioComponentFactoryFunction) -> AudioComponent

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

