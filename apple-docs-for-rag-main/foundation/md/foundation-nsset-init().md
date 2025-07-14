

- Foundation
- NSSet
-  init() 

Initializer

# init()

Initializes a newly allocated set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## Return Value

A set.

## Discussion

This method is a designated initializer of `NSSet`.

## See Also

### Initializing a Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(set: Set&lt;AnyHashable>)

Initializes a newly allocated set and adds to it objects from another given set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a newly allocated set and adds to it members of another given set.

