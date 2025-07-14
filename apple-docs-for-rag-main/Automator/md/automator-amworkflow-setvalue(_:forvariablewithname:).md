

- Automator
- AMWorkflow
-  setValue(\_:forVariableWithName:) 

Instance Method

# setValue(\_:forVariableWithName:)

Sets the value of the workflow variable with the specified name.

Mac Catalyst 14.0+macOS 10.4+

``` source
func setValue(
    _ value: Any?,
    forVariableWithName variableName: String
) -> Bool
```

## Parameters 

`value`  

The value to set for the named variable.

`variableName`  

The name of a variable to set the value for.

## Return Value

true if `variableName` was found and its value is set; otherwise false.

## Discussion

This method does nothing if the variable specified by `variableName` is not found.

