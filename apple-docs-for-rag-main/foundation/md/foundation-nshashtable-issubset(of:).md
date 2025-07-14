

- Foundation
- NSHashTable
-  isSubset(of:) 

Instance Method

# isSubset(of:)

Returns a Boolean value that indicates whether every element in the receiving hash table is also present in another given hash table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isSubset(of other: NSHashTable) -> Bool
```

## Parameters 

`other`  

The hash table with which to compare the receiving hash table.

## Return Value

true if every element in the receiving hash table is also present in `other`, otherwise false.

## Discussion

The equality test used for members depends on the personality option selected. For instance, choosing the objectPersonality option will use `isEqual:` to determine equality. See NSPointerFunctions.Options for more information on personality options and their corresponding equality tests.

## See Also

### Comparing Hash Tables

func intersect(NSHashTable&lt;ObjectType>)

Removes from the receiving hash table each element that isn’t a member of another given hash table.

func intersects(NSHashTable&lt;ObjectType>) -> Bool

Returns a Boolean value that indicates whether a given hash table intersects with the receiving hash table.

func isEqual(to: NSHashTable&lt;ObjectType>) -> Bool

Returns a Boolean value that indicates whether a given hash table is equal to the receiving hash table.

