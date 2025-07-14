

- Foundation
- NSCache
-  removeObject(forKey:) 

Instance Method

# removeObject(forKey:)

Removes the value of the specified key in the cache.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObject(forKey key: KeyType)
```

## Parameters 

`key`  

The key identifying the value to be removed.

## See Also

### Adding and Removing Cached Values

func setObject(ObjectType, forKey: KeyType)

Sets the value of the specified key in the cache.

func setObject(ObjectType, forKey: KeyType, cost: Int)

Sets the value of the specified key in the cache, and associates the key-value pair with the specified cost.

func removeAllObjects()

Empties the cache.

