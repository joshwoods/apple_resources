

- Quartz
- QCPlugIn
-  setValue(\_:forOutputKey:) Deprecated

Instance Method

# setValue(\_:forOutputKey:)

Sets the value of an output port.

macOS 10.4–10.15Deprecated

``` source
func setValue(
    _ value: Any!,
    forOutputKey key: String!
) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`value`  

The value to associate with the specified key.

`key`  

The key associated with the output port whose value you want to set.

## Return Value

true if successful; false if called outside of the execute(_:atTime:withArguments:) method.

## Discussion

You call this method from within your execute(_:atTime:withArguments:) method to set the output values of your custom patch.

## See Also

### Getting and Setting Port Values

func didValue(forInputKeyChange: String!) -> Bool

Returns whether the input port value changed since the last execution of the custom patch.

Deprecated

func value(forInputKey: String!) -> Any!

Returns the current value for an input port.

Deprecated

