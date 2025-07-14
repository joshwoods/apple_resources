

- ScreenCaptureKit
- SCStream
-  removeStreamOutput(\_:type:) 

Instance Method

# removeStreamOutput(\_:type:)

Removes a destination from receiving stream output.

Mac Catalyst 18.2+macOS 12.3+

``` source
func removeStreamOutput(
    _ output: any SCStreamOutput,
    type: SCStreamOutputType
) throws
```

## Parameters 

`output`  

The object to remove that conforms to the stream output protocol.

`type`  

The stream output type.

## See Also

### Adding and removing stream output

func addStreamOutput(any SCStreamOutput, type: SCStreamOutputType, sampleHandlerQueue: dispatch_queue_t?) throws

Adds a destination that receives the stream output.

