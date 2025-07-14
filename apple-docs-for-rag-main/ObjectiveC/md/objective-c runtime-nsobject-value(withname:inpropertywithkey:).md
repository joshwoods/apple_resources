

- Objective-C Runtime
- NSObject
-  value(withName:inPropertyWithKey:) 

Instance Method

# value(withName:inPropertyWithKey:)

Retrieves a named object from the collection specified by the passed key.

Mac CatalystmacOS

``` source
func value(
    withName name: String,
    inPropertyWithKey key: String
) -> Any?
```

## Discussion

The method `valueInWithName:` is used if it exists. Otherwise, raises an `NSUndefinedKeyException`.

## See Also

### Access by name, key, or ID

func insertValue(Any, inPropertyWithKey: String)

Inserts an object in the collection specified by the passed key.

func value(withUniqueID: Any, inPropertyWithKey: String) -> Any?

Retrieves an object by ID from the collection specified by the passed key.

