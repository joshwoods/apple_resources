

- Foundation
- NSCountedSet
-  init(set:) 

Initializer

# init(set:)

Returns a counted set object initialized with the contents of a given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(set: Set)
```

## Parameters 

`set`  

An set of objects to add to the new set.

## Return Value

An initialized counted set object with the contents of `set`. The returned object might be different than the original receiver.

## See Also

### Related Documentation

convenience init(set: Set&lt;AnyHashable>)

Initializes a newly allocated set and adds to it objects from another given set.

### Initializing a Counted Set

convenience init(array: [Any])

Returns a counted set object initialized with the contents of a given array.

init(capacity: Int)

Returns a counted set object initialized with enough memory to hold a given number of objects.

