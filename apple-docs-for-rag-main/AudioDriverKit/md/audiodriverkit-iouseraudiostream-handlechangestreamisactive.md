

- AudioDriverKit
- IOUserAudioStream
-  HandleChangeStreamIsActive 

Instance Method

# HandleChangeStreamIsActive

Tells the stream the activity state is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeStreamIsActive(bool in_is_active);
```

## Parameters 

`in_is_active`  

`true` if the stream is to become active; otherwise, `false`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetStreamIsActive and returns kIOReturnSuccess. Subclass and override this method to handle changes to the stream format and return kIOReturnSuccess upon success.

## See Also

### Managing Stream Changes

HandleChangeCurrentStreamFormat

Tells the stream the format is changing.

DeviceSampleRateChanged

Updates stream formats, in response to the owning audio device changing its sample rate.

