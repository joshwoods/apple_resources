

- ScreenCaptureKit
- SCStream
-  addStreamOutput(\_:type:sampleHandlerQueue:) 

Instance Method

# addStreamOutput(\_:type:sampleHandlerQueue:)

Adds a destination that receives the stream output.

Mac Catalyst 18.2+macOS 12.3+

``` source
func addStreamOutput(
    _ output: any SCStreamOutput,
    type: SCStreamOutputType,
    sampleHandlerQueue: dispatch_queue_t?
) throws
```

## Parameters 

`output`  

The object that conforms to the stream output protocol.

`type`  

The stream output type.

`sampleHandlerQueue`  

The queue that receives the stream output.

## Discussion

Use this method to attach an object that conforms to SCStreamOutput to receive stream content. Optionally, provide a DispatchQueue to send output to a queue that’s responsible for processing the output.

## See Also

### Adding and removing stream output

func removeStreamOutput(any SCStreamOutput, type: SCStreamOutputType) throws

Removes a destination from receiving stream output.

