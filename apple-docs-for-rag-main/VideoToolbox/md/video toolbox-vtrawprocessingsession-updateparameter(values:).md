

- Video Toolbox
- VTRAWProcessingSession
-  updateParameter(values:) 

Instance Method

# updateParameter(values:)

Sets the value for one or more of the processing parameters.

macOS 15.0+

``` source
func updateParameter(values: [String : Any]) throws
```

## Parameters 

`values`  

A dictionary where keys correspond to Parameter.details.key for the parameters being set, and the value is appropriate to the Parameter type This call will throw an error if the RAW Processor extension process is unreachable or if the provided parameter values are invalid or out of range

## See Also

### Configuring parameters

func parameters() -> any AsyncSequence&lt;[VTRAWProcessingSession.Parameter], Never>

Returns an asynchronous sequence that provides updates to the processing Parameter array if the processing extension makes changes to the set of Parameters.

var processingParameters: [VTRAWProcessingSession.Parameter]

An array of processing parameters available for this RAW processing session.

enum Parameter

A parameter expresses a control or a set of controls that influence frame processing.

