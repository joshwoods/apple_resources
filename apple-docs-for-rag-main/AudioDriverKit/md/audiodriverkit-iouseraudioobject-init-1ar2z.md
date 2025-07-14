

- AudioDriverKit
- IOUserAudioObject
-  init 

Instance Method

# init

Initializes an instance of the audio object base class.

DriverKit 21.0+

``` source
bool init(IOUserAudioDriver * in_audio_driver);
```

## Parameters 

`in_audio_driver`  

The IOUserAudioDriver that owns this object.

## Return Value

A Boolean value that indicates the result of initialization: `true` if initialization succeeded, `false` otherwise.

## Discussion

Always pass in the IOUserAudioDriver. The no-arg initializer, init, always returns `false`.

## See Also

### Creating an Audio Object

init

Initializes an empty object.

