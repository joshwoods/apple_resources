

- Foundation
- NSCountedSet
-  init(array:) 

Initializer

# init(array:)

Returns a counted set object initialized with the contents of a given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(array: [Any])
```

## Parameters 

`array`  

An array of objects to add to the new set.

## Return Value

An initialized counted set object with the contents of `array`. The returned object might be different than the original receiver.

## See Also

### Related Documentation

Collections Programming Topics

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

### Initializing a Counted Set

convenience init(set: Set&lt;AnyHashable>)

Returns a counted set object initialized with the contents of a given set.

init(capacity: Int)

Returns a counted set object initialized with enough memory to hold a given number of objects.

