

- Swift
- ManagedBufferPointer
-  capacity 

Instance Property

# capacity

The actual number of elements that can be stored in this object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var capacity: Int { get }
```

## Discussion

This value may be nontrivial to compute; it is usually a good idea to store this information in the “header” area when an instance is created.

## See Also

### Inspecting a Buffer

var header: Header

The stored `Header` instance.

var buffer: AnyObject

Returns the object instance being used for storage.

func isUniqueReference() -> Bool

Returns `true` if `self` holds the only strong reference to its buffer; otherwise, returns `false`.

