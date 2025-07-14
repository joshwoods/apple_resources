

- Swift
- UnsafePointer
-  deallocate() 

Instance Method

# deallocate()

Deallocates the memory block previously allocated at this pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deallocate()
```

## Discussion

This pointer must be a pointer to the start of a previously allocated memory block. The memory must not be initialized or `Pointee` must be a trivial type.

