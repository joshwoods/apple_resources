

- Foundation
- NSOrderedSet
-  init(objects:count:) 

Initializer

# init(objects:count:)

Creates and returns a set containing a specified number of objects from a given C array of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    objects: UnsafePointer,
    count cnt: Int
)
```

## Parameters 

`objects`  

A C array of objects to add to the new ordered set.

If the same object appears more than once in objects, it is added only once to the returned ordered set. Each object receives a retain message as it is added to the set.

`cnt`  

The number of objects from objects to add to the new set.

## Return Value

A new ordered set containing cnt objects from the list of objects specified by `objects`.

## See Also

### Related Documentation

convenience init(orderedSet: NSOrderedSet, copyItems: Bool)

Initializes a new ordered set with the contents of a set, optionally copying the items.

convenience init(orderedSet: NSOrderedSet)

Initializes a new ordered set with the contents of a set.

