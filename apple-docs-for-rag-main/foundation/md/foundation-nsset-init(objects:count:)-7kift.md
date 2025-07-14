

- Foundation
- NSSet
-  init(objects:count:) 

Initializer

# init(objects:count:)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    objects: UnsafePointer?,
    count cnt: Int
)
```

## Parameters 

`objects`  

A C array of objects to add to the new set. If the same object appears more than once in `objects`, it is added only once to the returned set. Each object receives a retain message as it is added to the set.

`cnt`  

The number of objects from `objects` to add to the new set.

## Return Value

An initialized set containing `cnt` objects from the list of objects specified by `objects`. The returned set might be different than the original receiver.

## Discussion

This method is a designated initializer for `NSSet`.

## See Also

### Related Documentation

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

### Initializing a Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

convenience init(set: Set&lt;AnyHashable>)

Initializes a newly allocated set and adds to it objects from another given set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a newly allocated set and adds to it members of another given set.

init()

Initializes a newly allocated set.

