

- AudioDriverKit
- IOUserAudioStream
-  HandleChangeCurrentStreamFormat 

Instance Method

# HandleChangeCurrentStreamFormat

Tells the stream the format is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeCurrentStreamFormat(const IOUserAudioStreamBasicDescription * in_format);
```

## Parameters 

`in_format`  

The stream format to set, if possible, as an `IOUserAudioStreamBasicDescription`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetCurrentStreamFormat and returns kIOReturnSuccess. Subclass and override this method to handle changes to the stream format and return kIOReturnSuccess upon success.

## See Also

### Managing Stream Changes

HandleChangeStreamIsActive

Tells the stream the activity state is changing.

DeviceSampleRateChanged

Updates stream formats, in response to the owning audio device changing its sample rate.

