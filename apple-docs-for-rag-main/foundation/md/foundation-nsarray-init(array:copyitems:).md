

- Foundation
- NSArray
-  init(array:copyItems:) 

Initializer

# init(array:copyItems:)

Initializes a newly allocated array using `anArray` as the source of data objects for the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    array: [Any],
    copyItems flag: Bool
)
```

## Parameters 

`array`  

An array containing the objects with which to initialize the new array.

`flag`  

If true, each object in `array` receives a copyWithZone: message to create a copy of the object—objects must conform to the `NSCopying` protocol. In a managed memory environment, this is instead of the `retain` message the object would otherwise receive. The object copy is then added to the returned array.

If false, then in a managed memory environment each object in `array` simply receives a `retain` message when it is added to the returned array.

## Return Value

An array initialized to contain the objects—or if `flag` is true, copies of the objects—in `array`. The returned object might be different than the original receiver.

## Discussion

After an immutable array has been initialized in this way, it cannot be modified.

The copy(with:) method performs a shallow copy. If you have a collection of arbitrary depth, passing true for the `flag` parameter will perform an immutable copy of the first level below the surface. If you pass false the mutability of the first level is unaffected. In either case, the mutability of all deeper levels is unaffected.

## See Also

### Related Documentation

convenience init(object: Any)

Creates and returns an array containing a given object.

### Initializing an Array

init()

Initializes a newly allocated array.

convenience init(array: [Any])

Initializes a newly allocated array by placing in it the objects contained in a given array.

convenience init?(contentsOfFile: String)

Initializes a newly allocated array with the contents of the file specified by a given path.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated array with the contents of the location specified by a given URL.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated array to include a given number of objects from a given C array.

