

- Foundation
- NSMutableArray
-  init(capacity:) 

Initializer

# init(capacity:)

Returns an array, initialized with enough memory to initially hold a given number of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(capacity numItems: Int)
```

## Parameters 

`numItems`  

The initial capacity of the new array.

## Return Value

An array initialized with enough memory to hold `numItems` objects. The returned object might be different than the original receiver.

## Discussion

Mutable arrays expand as needed; `numItems` simply establishes the object’s initial capacity.

This method is a designated initializer.

## See Also

### Creating and Initializing a Mutable Array

init?(contentsOfURL: URL)

Creates and returns a mutable array containing the contents specified by a given URL.

init()

Initializes a newly allocated array.

