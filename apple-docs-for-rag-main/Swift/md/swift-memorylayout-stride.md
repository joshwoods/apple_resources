

- Swift
- MemoryLayout
-  stride 

Type Property

# stride

The number of bytes from the start of one instance of `T` to the start of the next when stored in contiguous memory or in an `Array`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var stride: Int { get }
```

## Discussion

This is the same as the number of bytes moved when an `UnsafePointer` instance is incremented. `T` may have a lower minimal alignment that trades runtime performance for space efficiency. This value is always positive.

## See Also

### Accessing the Layout of a Type

static var size: Int

The contiguous memory footprint of `T`, in bytes.

static var alignment: Int

The default memory alignment of `T`, in bytes.

