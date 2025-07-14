

- Foundation
- NSCache
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the value associated with a given key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(forKey key: KeyType) -> ObjectType?
```

## Parameters 

`key`  

An object identifying the value.

## Return Value

The value associated with `key`, or `nil` if no value is associated with `key`.

## See Also

### Related Documentation

func removeObject(forKey: KeyType)

Removes the value of the specified key in the cache.

func setObject(ObjectType, forKey: KeyType, cost: Int)

Sets the value of the specified key in the cache, and associates the key-value pair with the specified cost.

func setObject(ObjectType, forKey: KeyType)

Sets the value of the specified key in the cache.

