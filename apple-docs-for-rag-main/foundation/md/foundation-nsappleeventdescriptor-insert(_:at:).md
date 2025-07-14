

- Foundation
- NSAppleEventDescriptor
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts a descriptor at the specified (one-based) position in the receiving descriptor list, replacing the existing descriptor, if any, at that position.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insert(
    _ descriptor: NSAppleEventDescriptor,
    at index: Int
)
```

## Parameters 

`descriptor`  

The descriptor to insert in the receiver. Specifying an index of 0 or count + 1 causes appending to the end of the list.

`index`  

The one-based descriptor list position at which to insert the descriptor.

## Discussion

Because it actually replaces the descriptor, if any, at the specified position, this method might better be called `replaceDescriptor:atIndex:`. The receiver must be a list descriptor. The indices are one-based. Currently provides no indication if an error occurs.

## See Also

### Working With List Descriptors

func atIndex(Int) -> NSAppleEventDescriptor?

Returns the descriptor at the specified (one-based) position in the receiving descriptor list.

func remove(at: Int)

Removes the descriptor at the specified (one-based) position in the receiving descriptor list.

