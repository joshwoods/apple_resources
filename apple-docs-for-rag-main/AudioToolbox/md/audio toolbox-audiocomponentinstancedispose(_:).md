

- Audio Toolbox
-  AudioComponentInstanceDispose(\_:) 

Function

# AudioComponentInstanceDispose(\_:)

Disposes of an audio component instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentInstanceDispose(_ inInstance: AudioComponentInstance) -> OSStatus
```

## Parameters 

`inInstance`  

The audio component instance that you want to dispose of.

## Return Value

A result code.

## See Also

### Creating an Audio Component Instance

func AudioComponentInstanceNew(AudioComponent, UnsafeMutablePointer&lt;AudioComponentInstance?>) -> OSStatus

Creates a new instance of an audio component.

func AudioComponentInstantiate(AudioComponent, AudioComponentInstantiationOptions, (AudioComponentInstance?, OSStatus) -> Void)

typealias AudioComponent

An audio component.

struct AudioComponentInstantiationOptions

Audio Component Errors

