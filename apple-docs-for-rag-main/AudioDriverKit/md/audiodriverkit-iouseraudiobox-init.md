

- AudioDriverKit
- IOUserAudioBox
-  init 

Instance Method

# init

Initializes an instance of the audio box class.

DriverKit 21.0+

``` source
bool init(IOUserAudioDriver * in_driver, bool in_is_acquirable, OSString * in_box_uid);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_is_acquirable`  

A Boolean value that specifies if the box supports being acquired.

`in_box_uid`  

The name of the box, as an OSString.

## Return Value

`true` if initialization succeeded; `false` otherwise.

## Discussion

Always pass in the IOUserAudioDriver and arguments. The no-argument \`\`IOUserAudioBox/init\`\`\`()`always returns`false\`.

## See Also

### Creating an Audio Box

Create

Allocates and initializes an instance of the audio box class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

