

- Audio Toolbox
- AUAudioUnit
-  instantiate(with:options:completionHandler:) 

Type Method

# instantiate(with:options:completionHandler:)

Asynchronously creates an audio unit instance.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func instantiate(
    with componentDescription: AudioComponentDescription,
    options: AudioComponentInstantiationOptions = [],
    completionHandler: @escaping (AUAudioUnit?, (any Error)?) -> Void
)
```

``` source
class func instantiate(
    with componentDescription: AudioComponentDescription,
    options: AudioComponentInstantiationOptions = []
) async throws -> AUAudioUnit
```

## Parameters 

`componentDescription`  

The component to instantiate.

`options`  

Options for loading the unit in-process or out-of-process.

`completionHandler`  

The block called when instantiation has completed. The block parameters are defined as follows:

audioUnit  
An initialized audio unit if the operation succeeded, or `nil` if it failed.

error  
An error if the operation failed, or `nil` if it succeeded.

## Discussion

Certain types of audio units must be instantiated asynchronously, such as version 3 units with a view.

Note

Do not block the main thread while waiting for the completion handler to be called; this can deadlock.

## See Also

### Creating an Audio Unit

convenience init(componentDescription: AudioComponentDescription) throws

Synchronously initializes a new audio unit object.

init(componentDescription: AudioComponentDescription, options: AudioComponentInstantiationOptions) throws

Synchronously initializes a new audio unit object.

