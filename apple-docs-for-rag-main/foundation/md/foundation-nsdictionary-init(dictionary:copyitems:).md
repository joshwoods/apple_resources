

- Foundation
- NSDictionary
-  init(dictionary:copyItems:) 

Initializer

# init(dictionary:copyItems:)

Initializes a newly allocated dictionary using the objects contained in another given dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    dictionary otherDictionary: [AnyHashable : Any],
    copyItems flag: Bool
)
```

## Parameters 

`otherDictionary`  

A dictionary containing the keys and values with which to initialize the new dictionary.

`flag`  

If true, each object in `otherDictionary` receives a copyWithZone: message to create a copy of the object—objects must conform to the `NSCopying` protocol. In a managed memory environment, this is instead of the `retain` message the object would otherwise receive. The object copy is then added to the returned dictionary.

If false, then in a managed memory environment each object in `otherDictionary` simply receives a `retain` message when it is added to the returned dictionary.

## Return Value

An initialized object—which might be different than the original receiver—containing the keys and values found in `otherDictionary`.

## Discussion

After an immutable dictionary has been initialized in this way, it cannot be modified.

The copy(with:) method performs a shallow copy. If you have a collection of arbitrary depth, passing true for the `flag` parameter will perform an immutable copy of the first level below the surface. If you pass false the mutability of the first level is unaffected. In either case, the mutability of all deeper levels is unaffected.

## See Also

### Creating a Dictionary from Another Dictionary

convenience init(dictionary: [AnyHashable : Any])

Initializes a newly allocated dictionary by placing in it the keys and values contained in another given dictionary.

