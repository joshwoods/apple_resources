

- Audio Toolbox
-  AudioComponentFindNext(\_:\_:) 

Function

# AudioComponentFindNext(\_:\_:)

Finds the next component that matches a specified `AudioComponentDescription` structure after a specified audio component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentFindNext(
    _ inComponent: AudioComponent?,
    _ inDesc: UnsafePointer
) -> AudioComponent?
```

## Parameters 

`inComponent`  

The audio component that you want to start searching after.

`inDesc`  

The description of the audio component you want to find.

## Return Value

An audio component, or nil if not found.

## See Also

### Creating an Audio Component Dynamically

func AudioComponentRegister(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioComponentFactoryFunction) -> AudioComponent

func AudioComponentCount(UnsafePointer&lt;AudioComponentDescription>) -> UInt32

Returns the number of audio components that match a specified `AudioComponentDescription` structure.

func AudioComponentInstanceGetComponent(AudioComponentInstance) -> AudioComponent

Retrieves a reference to an audio component from an instance of that audio component.

struct AudioComponentDescription

Identifying information for an audio component.

typealias AudioComponentInstance

A component instance, or object, is an audio unit or audio codec.

struct AudioComponentFlags

typealias AudioComponentFactoryFunction

