

- MediaExtension
- MERAWProcessorNotification
-  valuesDidChange 

Type Property

# valuesDidChange

A notification that indicates a change to the object’s set of available processing parameters.

macOS 15.0+

``` source
static let valuesDidChange: NSNotification.Name
```

## Discussion

This notification is used to notify the client that processor has changed the set of available MERAWProcessingParameter objects. This includes changing the set of available parameters, changing the enabled state for parameters, or changing default values for parameters. This may occur in response to incoming parameter changes, for example a change in a selected MERAWProcessingParameter.ListElement, or due to metadata-driven changes.

