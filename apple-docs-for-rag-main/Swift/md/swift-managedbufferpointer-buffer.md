

- Swift
- ManagedBufferPointer
-  buffer 

Instance Property

# buffer

Returns the object instance being used for storage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var buffer: AnyObject { get }
```

## See Also

### Inspecting a Buffer

var capacity: Int

The actual number of elements that can be stored in this object.

var header: Header

The stored `Header` instance.

func isUniqueReference() -> Bool

Returns `true` if `self` holds the only strong reference to its buffer; otherwise, returns `false`.

