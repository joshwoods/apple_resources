

- Quartz
- QCPlugIn
-  timeMode() Deprecated

Type Method

# timeMode()

Returns the time mode for the custom patch.

macOS 10.4–10.15Deprecated

``` source
class func timeMode() -> QCPlugInTimeMode
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The time mode of the custom patch. See QCPlugInTimeMode for the constants you can return.

## Discussion

You must implement this method to define whether you custom patch depends on time, doesn’t depend on time, or needs time to idle.

## See Also

### Defining the Characteristics of a Custom Patch

class func executionMode() -> QCPlugInExecutionMode

Returns the execution mode of the custom patch.

Deprecated

