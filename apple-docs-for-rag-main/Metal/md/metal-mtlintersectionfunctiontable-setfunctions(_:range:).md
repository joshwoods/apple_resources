

- Metal
- MTLIntersectionFunctionTable
-  setFunctions(\_:range:) 

Instance Method

# setFunctions(\_:range:)

Sets a range of entries in the table.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setFunctions(
    _ functions: [(any MTLFunctionHandle)?],
    range: Range
)
```

## Parameters 

`functions`  

The new entries for the table.

`range`  

A range of indices to change in the table.

## See Also

### Setting a Table Entry

func setFunction((any MTLFunctionHandle)?, index: Int)

Sets an entry in the table.

**Required**

