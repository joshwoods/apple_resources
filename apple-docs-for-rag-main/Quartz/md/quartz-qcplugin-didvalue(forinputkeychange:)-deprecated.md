

- Quartz
- QCPlugIn
-  didValue(forInputKeyChange:) Deprecated

Instance Method

# didValue(forInputKeyChange:)

Returns whether the input port value changed since the last execution of the custom patch.

macOS 10.4–10.15Deprecated

``` source
func didValue(forInputKeyChange key: String!) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The key for the input port whose value you want to check.

## Return Value

true if the value on the input port changed since the last time the execute(_:atTime:withArguments:) method was called; always returns false if called outside of the `execute:atTime:withArguments:` method.

## See Also

### Getting and Setting Port Values

func value(forInputKey: String!) -> Any!

Returns the current value for an input port.

Deprecated

func setValue(Any!, forOutputKey: String!) -> Bool

Sets the value of an output port.

Deprecated

