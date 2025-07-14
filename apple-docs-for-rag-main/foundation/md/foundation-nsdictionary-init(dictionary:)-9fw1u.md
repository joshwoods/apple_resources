

- Foundation
- NSDictionary
-  init(dictionary:) 

Initializer

# init(dictionary:)

Initializes a newly allocated dictionary by placing in it the keys and values contained in another given dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(dictionary otherDictionary: [AnyHashable : Any])
```

## Parameters 

`otherDictionary`  

A dictionary containing the keys and values with which to initialize the new dictionary.

## Return Value

An initialized dictionary—which might be different than the original receiver—containing the keys and values found in `otherDictionary`.

## See Also

### Creating a Dictionary from Another Dictionary

convenience init(dictionary: [AnyHashable : Any], copyItems: Bool)

Initializes a newly allocated dictionary using the objects contained in another given dictionary.

