

- AVFAudio
- AVAudioUnit
-  instantiate(with:options:completionHandler:) 

Type Method

# instantiate(with:options:completionHandler:)

Creates an instance of an audio unit component asynchronously and wraps it in an audio unit class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func instantiate(
    with audioComponentDescription: AudioComponentDescription,
    options: AudioComponentInstantiationOptions = [],
    completionHandler: @escaping (AVAudioUnit?, (any Error)?) -> Void
)
```

``` source
class func instantiate(
    with audioComponentDescription: AudioComponentDescription,
    options: AudioComponentInstantiationOptions = []
) async throws -> AVAudioUnit
```

## Parameters 

`audioComponentDescription`  

The component to create.

`options`  

The options the method uses to create the component.

`completionHandler`  

A handler the framework calls in an arbitrary thread context when creation completes. Retain the AVAudioUnit this handler provides.

## Discussion

You must create components with flags that include requiresAsyncInstantiation asynchronously through this method if they’re for use with AVAudioEngine.

The AVAudioUnit instance is usually a subclass that the method selects according to the components type. For example, AVAudioUnitEffect, AVAudioUnitGenerator, AVAudioUnitMIDIInstrument, or AVAudioUnitTimeEffect.

