

- Quartz
- QCPlugIn
-  executionMode() Deprecated

Type Method

# executionMode()

Returns the execution mode of the custom patch.

macOS 10.4–10.15Deprecated

``` source
class func executionMode() -> QCPlugInExecutionMode
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The execution mode of the custom patch. See QCPlugInExecutionMode for the constants you can return.

## Discussion

You must implement this method to define whether your custom patch is a provider, a processor, or a consumer.

## See Also

### Defining the Characteristics of a Custom Patch

class func timeMode() -> QCPlugInTimeMode

Returns the time mode for the custom patch.

Deprecated

