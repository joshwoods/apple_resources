

- Objective-C Runtime
- NSObject
-  value(at:inPropertyWithKey:) 

Instance Method

# value(at:inPropertyWithKey:)

Retrieves an indexed object from the collection specified by the passed key.

Mac CatalystmacOS

``` source
func value(
    at index: Int,
    inPropertyWithKey key: String
) -> Any?
```

## Discussion

This actually works with a single-value key as well if `index` is 0. The method `valueInAtIndex:` is used if it exists.

## See Also

### Indexed access

func insertValue(Any, at: Int, inPropertyWithKey: String)

Inserts an object at the specified index in the collection specified by the passed key.

func removeValue(at: Int, fromPropertyWithKey: String)

Removes the object at the specified index from the collection specified by the passed key.

func replaceValue(at: Int, inPropertyWithKey: String, withValue: Any)

Replaces the object at the specified index in the collection specified by the passed key.

