

- Foundation
- NSSet
-  init(set:) 

Initializer

# init(set:)

Initializes a newly allocated set and adds to it objects from another given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(set: Set)
```

## Parameters 

`set`  

A set containing objects to add to the receiving set. Each object is retained as it is added.

## Return Value

An initialized objects set containing the objects from `set`. The returned set might be different than the original receiver.

## See Also

### Initializing a Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a newly allocated set and adds to it members of another given set.

init()

Initializes a newly allocated set.

