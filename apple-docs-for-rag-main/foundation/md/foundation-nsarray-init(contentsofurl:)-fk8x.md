

- Foundation
- NSArray
-  init(contentsOfURL:) 

Initializer

# init(contentsOfURL:)

Creates and returns an array containing the contents specified by a given URL.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
init?(contentsOfURL url: URL)
```

## Parameters 

`url`  

The location of a file containing a string representation of an array produced by the write(to:atomically:) method.

## Return Value

An array containing the contents specified by `aURL`. Returns `nil` if the location can’t be opened or if the contents of the location can’t be parsed into an array.

## Discussion

The array representation at the location identified by `aURL` must contain only property list objects (`NSString`, `NSData`, `NSArray`, or `NSDictionary` objects). The objects contained by this array are immutable, even if the array is mutable.

## See Also

### Related Documentation

func write(to: URL, atomically: Bool) -> Bool

Writes the contents of the array to the location specified by a given URL.

### Creating an Array

convenience init(object: Any)

Creates and returns an array containing a given object.

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns an array that includes a given number of objects from a given C array.

