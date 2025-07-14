

- Foundation
- NSSet
-  init(set:copyItems:) 

Initializer

# init(set:copyItems:)

Initializes a newly allocated set and adds to it members of another given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    set: Set,
    copyItems flag: Bool
)
```

## Parameters 

`set`  

A set containing objects to add to the new set.

`flag`  

If true, each object in `set` receives a copyWithZone: message to create a copy of the object—objects must conform to the `NSCopying` protocol. In a managed memory environment, this is instead of the `retain` message the object would otherwise receive. The object copy is then added to the returned set.

If false, then in a managed memory environment each object in `set` simply receives a `retain` message when it is added to the returned set.

## Return Value

An initialized set that contains the members of `set`. The returned set might be different than the original receiver.

## Discussion

After an immutable s has been initialized in this way, it cannot be modified.

The copy(with:) method performs a shallow copy. If you have a collection of arbitrary depth, passing true for the `flag` parameter will perform an immutable copy of the first level below the surface. If you pass false the mutability of the first level is unaffected. In either case, the mutability of all deeper levels is unaffected.

## See Also

### Initializing a Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(set: Set&lt;AnyHashable>)

Initializes a newly allocated set and adds to it objects from another given set.

init()

Initializes a newly allocated set.

