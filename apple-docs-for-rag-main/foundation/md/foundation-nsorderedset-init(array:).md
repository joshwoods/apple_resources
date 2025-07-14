

- Foundation
- NSOrderedSet
-  init(array:) 

Initializer

# init(array:)

Initializes a newly allocated set with the objects that are contained in a given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(array: [Any])
```

## Parameters 

`array`  

An array of objects to add to the new set.

If the same object appears more than once in array, it is represented only once in the returned ordered set.

## Return Value

An initialized ordered set with the contents of array. The returned ordered set might be different than the original receiver.

## See Also

### Initializing an Ordered Set

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

