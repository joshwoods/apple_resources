

- Foundation
- NSFastEnumeration
-  countByEnumerating(with:objects:count:) 

Instance Method

# countByEnumerating(with:objects:count:)

Returns by reference a C array of objects over which the sender should iterate, and as the return value the number of objects in the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func countByEnumerating(
    with state: UnsafeMutablePointer,
    objects buffer: AutoreleasingUnsafeMutablePointer,
    count len: Int
) -> Int
```

**Required**

## Parameters 

`state`  

Context information that is used in the enumeration to, in addition to other possibilities, ensure that the collection has not been mutated.

`buffer`  

A C array of objects over which the sender is to iterate.

`len`  

The maximum number of objects to return in `stackbuf`.

## Return Value

The number of objects returned in `stackbuf`. Returns `0` when the iteration is finished.

## Discussion

The state structure is assumed to be of stack local memory, so you can recast the passed in state structure to one more suitable for your iteration.

