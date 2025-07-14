

- Foundation
- NSSet
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

An array of objects to add to the new set. If the same object appears more than once in `array`, it is represented only once in the returned set. Each object receives a retain message as it is added to the set.

## Return Value

An initialized set with the contents of `array`. The returned set might be different than the original receiver.

## See Also

### Initializing a Set

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(set: Set&lt;AnyHashable>)

Initializes a newly allocated set and adds to it objects from another given set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a newly allocated set and adds to it members of another given set.

init()

Initializes a newly allocated set.

