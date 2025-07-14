

- Swift
- UnsafeRawPointer
-  deallocate() 

Instance Method

# deallocate()

Deallocates the previously allocated memory block referenced by this pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deallocate()
```

## Discussion

The memory to be deallocated must be uninitialized or initialized to a trivial type.

