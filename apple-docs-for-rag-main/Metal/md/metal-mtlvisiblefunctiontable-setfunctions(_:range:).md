

- Metal
- MTLVisibleFunctionTable
-  setFunctions(\_:range:) 

Instance Method

# setFunctions(\_:range:)

Sets a range of table entries to point to an array of callable functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setFunctions(
    _ functions: [(any MTLFunctionHandle)?],
    range: Range
)
```

## Parameters 

`functions`  

An array of function handles for the functions to be called.

`range`  

A range of indices to change in the table.

## See Also

### Setting a Table Entry

func setFunction((any MTLFunctionHandle)?, index: Int)

Sets a table entry to point to a callable function.

**Required**

