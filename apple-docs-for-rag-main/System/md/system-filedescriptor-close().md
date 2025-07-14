

- System
- FileDescriptor
-  close() 

Instance Method

# close()

Deletes a file descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func close() throws
```

## Mentioned in 

Adopting Swift File Operations

## Discussion

Deletes the file descriptor from the per-process object reference table. If this is the last reference to the underlying object, the object will be deactivated.

The corresponding C function is `close`.

## See Also

### Closing a File

func closeAfter&lt;R>(() throws -> R) throws -> R

Runs a closure and then closes the file descriptor, even if an error occurs.

