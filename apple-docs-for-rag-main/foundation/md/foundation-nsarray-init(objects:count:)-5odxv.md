

- Foundation
- NSArray
-  init(objects:count:) 

Initializer

# init(objects:count:)

Initializes a newly allocated array to include a given number of objects from a given C array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    objects: UnsafePointer?,
    count cnt: Int
)
```

## Parameters 

`objects`  

A C array of objects.

`cnt`  

The number of values from the `objects` C array to include in the new array. This number will be the count of the new array—it must not be negative or greater than the number of elements in `objects`.

## Return Value

A newly allocated array including the first `count` objects from `objects`. The returned object might be different than the original receiver.

## Discussion

Elements are added to the new array in the same order they appear in `objects`, up to but not including index `count`.

After an immutable array has been initialized in this way, it can’t be modified.

This method is a designated initializer.

## See Also

### Initializing an Array

init()

Initializes a newly allocated array.

convenience init(array: [Any])

Initializes a newly allocated array by placing in it the objects contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated array using `anArray` as the source of data objects for the array.

convenience init?(contentsOfFile: String)

Initializes a newly allocated array with the contents of the file specified by a given path.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated array with the contents of the location specified by a given URL.

