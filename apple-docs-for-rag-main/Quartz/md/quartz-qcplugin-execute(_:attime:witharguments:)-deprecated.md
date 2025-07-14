

- Quartz
- QCPlugIn
-  execute(\_:atTime:withArguments:) Deprecated

Instance Method

# execute(\_:atTime:withArguments:)

Performs the processing or rendering tasks appropriate for the custom patch.

macOS 10.4–10.15Deprecated

``` source
func execute(
    _ context: (any QCPlugInContext)!,
    atTime time: TimeInterval,
    withArguments arguments: [AnyHashable : Any]!
) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`context`  

An opaque object , conforming to the QCPlugInContext protocol, that represents the execution context of the `QCPlugIn` object. Do not retain this object or use it outside of the scope of this method.

`time`  

The execution interval.

`arguments`  

A dictionary of arguments that can be used during execution. See Execution Arguments.

## Return Value

false indicates the custom patch was not able to execute successfully. In this case, the Quartz Composer engine stops rendering the current frame.

## Discussion

The Quartz Composer engine calls this method each time your custom patch needs to execute. You must implement this method. The method should perform whatever tasks are appropriate for the custom patch, such as:

- reading values from the input ports

- computing output values

- updating the values on the output ports

- rendering to the execution context

For example implementations of this method, see Quartz Composer Custom Patch Programming Guide.

