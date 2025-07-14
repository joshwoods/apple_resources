

- Video Toolbox
- VTRAWProcessingSession
-  processingParameters 

Instance Property

# processingParameters

An array of processing parameters available for this RAW processing session.

macOS 15.0+

``` source
var processingParameters: [VTRAWProcessingSession.Parameter] { get throws }
```

## Discussion

This call throws an error if the RAW Processor extension process is unreachable.

## See Also

### Configuring parameters

func parameters() -> any AsyncSequence&lt;[VTRAWProcessingSession.Parameter], Never>

Returns an asynchronous sequence that provides updates to the processing Parameter array if the processing extension makes changes to the set of Parameters.

func updateParameter(values: [String : Any]) throws

Sets the value for one or more of the processing parameters.

enum Parameter

A parameter expresses a control or a set of controls that influence frame processing.

