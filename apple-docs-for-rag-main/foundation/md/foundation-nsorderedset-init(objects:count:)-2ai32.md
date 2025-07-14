

- Foundation
- NSOrderedSet
-  init(objects:count:) 

Initializer

# init(objects:count:)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    objects: UnsafePointer?,
    count cnt: Int
)
```

## Parameters 

`objects`  

A C array of objects to add to the new set.

If the same object appears more than once in objects, it is added only once to the returned ordered set.

`cnt`  

The number of objects from objects to add to the new ordered set.

## Return Value

An initialized ordered set containing cnt objects from the list of objects specified by objects. The returned set might be different than the original receiver.

## Discussion

This method is a designated initializer of `NSOrderedSet`.

## See Also

### Related Documentation

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

### Initializing an Ordered Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated set with the objects that are contained in a given array, optionally copying the items.

convenience init(array: [Any], range: NSRange, copyItems: Bool)

Initializes a newly allocated set with the objects that are contained in the specified range of an array, optionally copying the items.

convenience init(object: Any)

Initializes a new ordered set with the object.

convenience init(orderedSet: NSOrderedSet)

Initializes a new ordered set with the contents of a set.

convenience init(orderedSet: NSOrderedSet, copyItems: Bool)

Initializes a new ordered set with the contents of a set, optionally copying the items.

convenience init(orderedSet: NSOrderedSet, range: NSRange, copyItems: Bool)

Initializes a new ordered set with the contents of an ordered set, optionally copying the items.

convenience init(set: Set&lt;AnyHashable>)

Initializes a new ordered set with the contents of a set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a new ordered set with the contents of a set, optionally copying the objects in the set.

init()

Initializes a newly allocated ordered set.

