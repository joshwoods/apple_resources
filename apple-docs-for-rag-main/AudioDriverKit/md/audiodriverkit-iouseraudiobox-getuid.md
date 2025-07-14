

- AudioDriverKit
- IOUserAudioBox
-  GetUID 

Instance Method

# GetUID

Returns the UID of the audio box.

DriverKit 21.0+

``` source
OSSharedPtr GetUID();
```

## Return Value

The UID of the audio box.

## Discussion

This method synchronizes by using the work queue created by the object.

