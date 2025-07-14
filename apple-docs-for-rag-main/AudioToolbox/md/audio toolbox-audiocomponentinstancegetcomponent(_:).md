

- Audio Toolbox
-  AudioComponentInstanceGetComponent(\_:) 

Function

# AudioComponentInstanceGetComponent(\_:)

Retrieves a reference to an audio component from an instance of that audio component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentInstanceGetComponent(_ inInstance: AudioComponentInstance) -> AudioComponent
```

## Parameters 

`inInstance`  

The component instance whose corresponding factory object you want to get. Must not be `NULL`, and you must own the instance (specifically, you must not have previously called AudioComponentInstanceDispose(_:) on the instance).

## Return Value

A reference to the desired audio component. If the value provided in the `inInstance` parameter is invalid, returns `NULL`.

## Discussion

Use this function to retrieve a reference to the audio component that was used to instantiate a given audio component instance. You can then query the component for its attributes by calling the AudioComponentGetDescription(_:_:) function.

## See Also

### Creating an Audio Component Dynamically

func AudioComponentRegister(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioComponentFactoryFunction) -> AudioComponent

func AudioComponentCount(UnsafePointer&lt;AudioComponentDescription>) -> UInt32

Returns the number of audio components that match a specified `AudioComponentDescription` structure.

func AudioComponentFindNext(AudioComponent?, UnsafePointer&lt;AudioComponentDescription>) -> AudioComponent?

Finds the next component that matches a specified `AudioComponentDescription` structure after a specified audio component.

struct AudioComponentDescription

Identifying information for an audio component.

typealias AudioComponentInstance

A component instance, or object, is an audio unit or audio codec.

struct AudioComponentFlags

typealias AudioComponentFactoryFunction

