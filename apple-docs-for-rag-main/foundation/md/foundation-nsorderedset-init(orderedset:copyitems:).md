

- Foundation
- NSOrderedSet
-  init(orderedSet:copyItems:) 

Initializer

# init(orderedSet:copyItems:)

Initializes a new ordered set with the contents of a set, optionally copying the items.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    orderedSet set: NSOrderedSet,
    copyItems flag: Bool
)
```

## Parameters 

`set`  

A set.

`flag`  

If true the objects are copied to the ordered set; otherwise false.

## Return Value

An initialized ordered set containing the objects in the set.

## See Also

### Initializing an Ordered Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated set with the objects that are contained in a given array, optionally copying the items.

convenience init(array: [Any], range: NSRange, copyItems: Bool)

Initializes a newly allocated set with the objects that are contained in the specified range of an array, optionally copying the items.

convenience init(object: Any)

Initializes a new ordered set with the object.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(orderedSet: NSOrderedSet)

Initializes a new ordered set with the contents of a set.

convenience init(orderedSet: NSOrderedSet, range: NSRange, copyItems: Bool)

Initializes a new ordered set with the contents of an ordered set, optionally copying the items.

convenience init(set: Set&lt;AnyHashable>)

Initializes a new ordered set with the contents of a set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a new ordered set with the contents of a set, optionally copying the objects in the set.

init()

Initializes a newly allocated ordered set.

