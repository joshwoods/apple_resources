

- Foundation
- NSMapTable
-  removeObject(forKey:) 

Instance Method

# removeObject(forKey:)

Removes a given key and its associated value from the map table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObject(forKey aKey: KeyType?)
```

## Parameters 

`aKey`  

The key to remove.

## Discussion

Does nothing if `aKey` does not exist.

## See Also

### Manipulating Content

func setObject(ObjectType?, forKey: KeyType?)

Adds a given key-value pair to the map table.

func removeAllObjects()

Empties the map table of its entries.

