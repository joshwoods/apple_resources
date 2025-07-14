

- Automator
- AMWorkflow
-  valueForVariable(withName:) 

Instance Method

# valueForVariable(withName:)

Returns the value of the workflow variable with the specified name.

Mac Catalyst 14.0+macOS 10.4+

``` source
func valueForVariable(withName variableName: String) -> Any?
```

## Parameters 

`variableName`  

The variable name.

## Return Value

The value for the variable. Returns `nil` if no variable is found with the specified name.

## See Also

### Getting Information About a Workflow

var actions: [AMAction]

An array of the workflow’s actions.

var fileURL: URL?

A URL that specifies the location of the workflow file.

