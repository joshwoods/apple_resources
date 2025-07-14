

- Foundation
- NSMutableDictionary
-  init(capacity:) 

Initializer

# init(capacity:)

Initializes a newly allocated mutable dictionary, allocating enough memory to hold `numItems` entries.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(capacity numItems: Int)
```

## Parameters 

`numItems`  

The initial capacity of the initialized dictionary.

## Return Value

An initialized mutable dictionary, which might be different than the original receiver.

## Discussion

Mutable dictionaries allocate additional memory as needed, so `numItems` simply establishes the object’s initial capacity.

This method is a designated initializer of `NSMutableDictionary`.

## See Also

### Creating and Initializing a Mutable Dictionary

init()

Initializes a newly allocated mutable dictionary.

init(sharedKeySet: Any)

Creates a mutable dictionary which is optimized for dealing with a known set of keys.

