

- Metal
- MTLBuffer
-  didModifyRange(\_:) 

Instance Method

# didModifyRange(\_:)

Informs the GPU that the CPU has modified a section of the buffer.

Mac Catalyst 14.0+macOS 10.11+

``` source
func didModifyRange(_ range: Range)
```

## Parameters 

`range`  

The range of bytes that have been modified.

## Discussion

If you write information to a buffer created with the MTLStorageMode.managed storage mode, you must call this method to inform the GPU that the information has changed. If you execute GPU commands that read the data without calling this method first, the behavior is undefined.

