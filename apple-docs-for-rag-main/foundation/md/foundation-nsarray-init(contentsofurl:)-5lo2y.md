

- Foundation
- NSArray
-  init(contentsOfURL:) 

Initializer

# init(contentsOfURL:)

Initializes a newly allocated array with the contents of the location specified by a given URL.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
convenience init?(contentsOfURL url: URL)
```

``` source
convenience init?(contentsOf url: URL)
```

## Parameters 

`url`  

The location of a file containing a string representation of an array produced by the write(to:atomically:) method.

## Return Value

An array initialized to contain the contents specified by `aURL`. Returns `nil` if the location can’t be opened or if the contents of the location can’t be parsed into an array. The returned object might be different than the original receiver.

## Discussion

The array representation at the location identified by `aURL` must contain only property list objects (`NSString`, `NSData`, `NSArray`, or `NSDictionary` objects). The objects contained by this array are immutable, even if the array is mutable.

## See Also

### Related Documentation

init?(contentsOfURL: URL)

Creates and returns an array containing the contents specified by a given URL.

func write(to: URL, atomically: Bool) -> Bool

Writes the contents of the array to the location specified by a given URL.

### Initializing an Array

init()

Initializes a newly allocated array.

convenience init(array: [Any])

Initializes a newly allocated array by placing in it the objects contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated array using `anArray` as the source of data objects for the array.

convenience init?(contentsOfFile: String)

Initializes a newly allocated array with the contents of the file specified by a given path.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated array to include a given number of objects from a given C array.

