

- XPC
-  xpc_fd_dup(\_:) 

Function

# xpc_fd_dup(\_:)

Returns a file descriptor that is equivalent to the one that the specified file descriptor object boxes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_fd_dup(_ xfd: xpc_object_t) -> Int32
```

## Parameters 

`xfd`  

The file descriptor object which is to be examined.

## Return Value

A file descriptor that is equivalent to the one originally given to xpc_fd_create(_:). If the descriptor could not be created, -1 is returned.

## Discussion

Multiple invocations of xpc_fd_dup(_:) will not return the same file descriptor number, but they will return descriptors that are equivalent, as though they had been created by `dup(2)`.

The caller is responsible for calling `close(2)` on the returned descriptor.

## See Also

### File Descriptor objects

func xpc_fd_create(Int32) -> xpc_object_t?

Creates an XPC object that represents a POSIX file descriptor.

