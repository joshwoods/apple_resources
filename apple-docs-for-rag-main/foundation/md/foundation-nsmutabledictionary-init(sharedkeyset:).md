

- Foundation
- NSMutableDictionary
-  init(sharedKeySet:) 

Initializer

# init(sharedKeySet:)

Creates a mutable dictionary which is optimized for dealing with a known set of keys.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(sharedKeySet keyset: Any)
```

## Parameters 

`keyset`  

The `keyset`, created by the NSDictionary class method sharedKeySet(forKeys:).

Important

If `keyset` is `nil`, an exception is raised. If `keyset` is not an object returned by sharedKeySet(forKeys:), an exception is raised.

## Return Value

A new mutable dictionary optimized for a known set of keys.

## Discussion

Keys that are not in the key set can still be set in the dictionary, but that usage is not optimal.

## See Also

### Creating and Initializing a Mutable Dictionary

init(capacity: Int)

Initializes a newly allocated mutable dictionary, allocating enough memory to hold `numItems` entries.

init()

Initializes a newly allocated mutable dictionary.

