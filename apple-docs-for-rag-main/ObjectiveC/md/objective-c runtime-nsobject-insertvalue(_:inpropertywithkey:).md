

- Objective-C Runtime
- NSObject
-  insertValue(\_:inPropertyWithKey:) 

Instance Method

# insertValue(\_:inPropertyWithKey:)

Inserts an object in the collection specified by the passed key.

Mac CatalystmacOS

``` source
func insertValue(
    _ value: Any,
    inPropertyWithKey key: String
)
```

## Discussion

The method `insertIn:` is used if it exists. Otherwise, raises an `NSUndefinedKeyException`. This is part of Cocoa’s scripting support for inserting newly-created objects into containers without explicitly specifying a location.

## See Also

### Access by name, key, or ID

func value(withName: String, inPropertyWithKey: String) -> Any?

Retrieves a named object from the collection specified by the passed key.

func value(withUniqueID: Any, inPropertyWithKey: String) -> Any?

Retrieves an object by ID from the collection specified by the passed key.

