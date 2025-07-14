

- Objective-C Runtime
- NSObject
-  value(withUniqueID:inPropertyWithKey:) 

Instance Method

# value(withUniqueID:inPropertyWithKey:)

Retrieves an object by ID from the collection specified by the passed key.

Mac CatalystmacOS

``` source
func value(
    withUniqueID uniqueID: Any,
    inPropertyWithKey key: String
) -> Any?
```

## Discussion

The method `valueInWithUniqueID:` is invoked if it exists. Otherwise, raises an `NSUndefinedKeyException`. The declared type of `uniqueID` in the constructed method must be `id`, `NSNumber *`, `NSString *`, or one of the scalar types that can be encapsulated by `NSNumber`.

## See Also

### Access by name, key, or ID

func insertValue(Any, inPropertyWithKey: String)

Inserts an object in the collection specified by the passed key.

func value(withName: String, inPropertyWithKey: String) -> Any?

Retrieves a named object from the collection specified by the passed key.

