

- Foundation
- NSAppleEventDescriptor
-  atIndex(\_:) 

Instance Method

# atIndex(\_:)

Returns the descriptor at the specified (one-based) position in the receiving descriptor list.

Mac Catalyst 13.0+macOS 10.0+

``` source
func atIndex(_ index: Int) -> NSAppleEventDescriptor?
```

## Parameters 

`index`  

The one-based descriptor list position of the descriptor to return.

## Return Value

The descriptor from the specified position (one-based) in the descriptor list, or `nil` if the specified descriptor cannot be obtained.

## See Also

### Working With List Descriptors

func insert(NSAppleEventDescriptor, at: Int)

Inserts a descriptor at the specified (one-based) position in the receiving descriptor list, replacing the existing descriptor, if any, at that position.

func remove(at: Int)

Removes the descriptor at the specified (one-based) position in the receiving descriptor list.

