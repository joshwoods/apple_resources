

- AppKit
- NSTreeNode
-  sort(with:recursively:) 

Instance Method

# sort(with:recursively:)

Sorts the receiver’s subtree using the values of the represented objects with the specified sort descriptors.

macOS 10.5+

``` source
func sort(
    with sortDescriptors: [NSSortDescriptor],
    recursively: Bool
)
```

## Parameters 

`sortDescriptors`  

Array of sort descriptors specifying how to sort the represented objects.

`recursively`  

A Boolean that specifies whether the child nodes should be sorted recursively.

## Discussion

All the represented objects in the child nodes must be key-value coding compliant for the keys specified in the sort descriptors.

