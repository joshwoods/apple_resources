

- Foundation
- NSAppleEventDescriptor
-  remove(at:) 

Instance Method

# remove(at:)

Removes the descriptor at the specified (one-based) position in the receiving descriptor list.

Mac Catalyst 13.0+macOS 10.0+

``` source
func remove(at index: Int)
```

## Parameters 

`index`  

The one-based position of the descriptor to remove.

## Discussion

The receiver must be a list descriptor. The indices are one-based. Currently provides no indication if an error occurs.

## See Also

### Working With List Descriptors

func atIndex(Int) -> NSAppleEventDescriptor?

Returns the descriptor at the specified (one-based) position in the receiving descriptor list.

func insert(NSAppleEventDescriptor, at: Int)

Inserts a descriptor at the specified (one-based) position in the receiving descriptor list, replacing the existing descriptor, if any, at that position.

