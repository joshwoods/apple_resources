

- Quartz
- QCPlugIn
-  value(forInputKey:) Deprecated

Instance Method

# value(forInputKey:)

Returns the current value for an input port.

macOS 10.4–10.15Deprecated

``` source
func value(forInputKey key: String!) -> Any!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The key for the input port you want to check.

## Return Value

The value associated with the key or `nil` if called outside of the execute(_:atTime:withArguments:) method.

## Discussion

You call this method from within your execute(_:atTime:withArguments:) method to retrieve the input values of your custom patch.

## See Also

### Getting and Setting Port Values

func didValue(forInputKeyChange: String!) -> Bool

Returns whether the input port value changed since the last execution of the custom patch.

Deprecated

func setValue(Any!, forOutputKey: String!) -> Bool

Sets the value of an output port.

Deprecated

