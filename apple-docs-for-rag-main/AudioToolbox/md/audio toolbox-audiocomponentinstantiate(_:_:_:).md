

- Audio Toolbox
-  AudioComponentInstantiate(\_:\_:\_:) 

Function

# AudioComponentInstantiate(\_:\_:\_:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentInstantiate(
    _ inComponent: AudioComponent,
    _ inOptions: AudioComponentInstantiationOptions,
    _ inCompletionHandler: @escaping (AudioComponentInstance?, OSStatus) -> Void
)
```

## Mentioned in 

Hosting Audio Unit Extensions Using the AUv2 API

## See Also

### Creating an Audio Component Instance

func AudioComponentInstanceNew(AudioComponent, UnsafeMutablePointer&lt;AudioComponentInstance?>) -> OSStatus

Creates a new instance of an audio component.

func AudioComponentInstanceDispose(AudioComponentInstance) -> OSStatus

Disposes of an audio component instance.

typealias AudioComponent

An audio component.

struct AudioComponentInstantiationOptions

Audio Component Errors

