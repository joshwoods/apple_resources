

- Metal
- MTLVisibleFunctionTable
-  setFunction(\_:index:) 

Instance Method

# setFunction(\_:index:)

Sets a table entry to point to a callable function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setFunction(
    _ function: (any MTLFunctionHandle)?,
    index: Int
)
```

**Required**

## Parameters 

`function`  

A function handle for the function to be called.

`index`  

The index of the table entry to change.

## See Also

### Setting a Table Entry

func setFunctions([(any MTLFunctionHandle)?], range: Range&lt;Int>)

Sets a range of table entries to point to an array of callable functions.

