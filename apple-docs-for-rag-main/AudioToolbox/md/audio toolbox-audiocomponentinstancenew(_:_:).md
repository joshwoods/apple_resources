

- Audio Toolbox
-  AudioComponentInstanceNew(\_:\_:) 

Function

# AudioComponentInstanceNew(\_:\_:)

Creates a new instance of an audio component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentInstanceNew(
    _ inComponent: AudioComponent,
    _ outInstance: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inComponent`  

The audio component that you want to create a new instance of.

`outInstance`  

On output, the new audio component instance.

## Return Value

A result code.

## Mentioned in 

Hosting Audio Unit Extensions Using the AUv2 API

## See Also

### Creating an Audio Component Instance

func AudioComponentInstantiate(AudioComponent, AudioComponentInstantiationOptions, (AudioComponentInstance?, OSStatus) -> Void)

func AudioComponentInstanceDispose(AudioComponentInstance) -> OSStatus

Disposes of an audio component instance.

typealias AudioComponent

An audio component.

struct AudioComponentInstantiationOptions

Audio Component Errors

