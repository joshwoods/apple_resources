

- Foundation
- NSArray
-  init(objects:count:) 

Initializer

# init(objects:count:)

Creates and returns an array that includes a given number of objects from a given C array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    objects: UnsafePointer,
    count cnt: Int
)
```

## Parameters 

`objects`  

A C array of objects.

`cnt`  

The number of values from the `objects` C array to include in the new array. This number will be the count of the new array—it must not be negative or greater than the number of elements in `objects`.

## Return Value

A new array including the first `count` objects from `objects`.

## Discussion

Elements are added to the new array in the same order they appear in `objects`, up to but not including index `count`. For example:

```
NSString *strings[3];
strings[0] = @"First";
strings[1] = @"Second";
strings[2] = @"Third";

NSArray *stringsArray = [NSArray arrayWithObjects:strings count:2];
// strings array contains { @"First", @"Second" }
```

## See Also

### Creating an Array

init?(contentsOfURL: URL)

Creates and returns an array containing the contents specified by a given URL.

convenience init(object: Any)

Creates and returns an array containing a given object.

