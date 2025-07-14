

- Metal
- MTLBuffer
-  contents() 

Instance Method

# contents()

Gets the system address of the buffer’s storage allocation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func contents() -> UnsafeMutableRawPointer
```

**Required**

## Return Value

A pointer to the shared copy of the buffer data, or `NULL` for buffers allocated with a private resource storage mode (MTLStorageMode.private).

## Discussion

Private resources are not CPU-accessible.

