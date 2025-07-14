

- Video Toolbox
- VTRAWProcessingSession
-  parameters() 

Instance Method

# parameters()

Returns an asynchronous sequence that provides updates to the processing Parameter array if the processing extension makes changes to the set of Parameters.

macOS 15.0+

``` source
func parameters() -> any AsyncSequence
```

## Discussion

These changes could be: - adding or removing Parameters - enabling/disabling Parameters - changing default values for a Parameter

## See Also

### Configuring parameters

func updateParameter(values: [String : Any]) throws

Sets the value for one or more of the processing parameters.

var processingParameters: [VTRAWProcessingSession.Parameter]

An array of processing parameters available for this RAW processing session.

enum Parameter

A parameter expresses a control or a set of controls that influence frame processing.

