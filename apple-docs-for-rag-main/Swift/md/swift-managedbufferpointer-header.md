

- Swift
- ManagedBufferPointer
-  header 

Instance Property

# header

The stored `Header` instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var header: Header { get set }
```

## See Also

### Inspecting a Buffer

var capacity: Int

The actual number of elements that can be stored in this object.

var buffer: AnyObject

Returns the object instance being used for storage.

func isUniqueReference() -> Bool

Returns `true` if `self` holds the only strong reference to its buffer; otherwise, returns `false`.

