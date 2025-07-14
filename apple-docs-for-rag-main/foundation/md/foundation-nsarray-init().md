

- Foundation
- NSArray
-  init() 

Initializer

# init()

Initializes a newly allocated array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## Return Value

An array.

## Discussion

After an immutable array has been initialized in this way, it cannot be modified.

This method is a designated initializer.

## See Also

### Initializing an Array

convenience init(array: [Any])

Initializes a newly allocated array by placing in it the objects contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated array using `anArray` as the source of data objects for the array.

convenience init?(contentsOfFile: String)

Initializes a newly allocated array with the contents of the file specified by a given path.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated array with the contents of the location specified by a given URL.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated array to include a given number of objects from a given C array.

