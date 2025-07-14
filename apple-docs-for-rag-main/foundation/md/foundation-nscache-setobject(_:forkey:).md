

- Foundation
- NSCache
-  setObject(\_:forKey:) 

Instance Method

# setObject(\_:forKey:)

Sets the value of the specified key in the cache.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setObject(
    _ obj: ObjectType,
    forKey key: KeyType
)
```

## Parameters 

`obj`  

The object to be stored in the cache.

`key`  

The key with which to associate the value.

## Discussion

Unlike an `NSMutableDictionary` object, a cache does not copy the key objects that are put into it.

## See Also

### Adding and Removing Cached Values

func setObject(ObjectType, forKey: KeyType, cost: Int)

Sets the value of the specified key in the cache, and associates the key-value pair with the specified cost.

func removeObject(forKey: KeyType)

Removes the value of the specified key in the cache.

func removeAllObjects()

Empties the cache.

