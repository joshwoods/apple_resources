

- Foundation
- NSHashTable
-  union(\_:) 

Instance Method

# union(\_:)

Adds each element in another given hash table to the receiving hash table, if not present.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func union(_ other: NSHashTable)
```

## Parameters 

`other`  

The hash table of elements to add to the receiving hash table.

## Discussion

The equality test used for members depends on the personality option selected. For instance, choosing the objectPersonality option will use `isEqual:` to determine equality. See NSPointerFunctions.Options for more information on personality options and their corresponding equality tests.

## See Also

### Set Functions

func minus(NSHashTable&lt;ObjectType>)

Removes each element in another given hash table from the receiving hash table, if present.

