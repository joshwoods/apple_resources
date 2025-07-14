

- Foundation
- NSMutableDictionary
-  removeObjects(forKeys:) 

Instance Method

# removeObjects(forKeys:)

Removes from the dictionary entries specified by elements in a given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObjects(forKeys keyArray: [Any])
```

## Parameters 

`keyArray`  

An array of objects specifying the keys to remove.

## Discussion

If a key in `keyArray` does not exist, the entry is ignored.

## See Also

### Removing Entries From a Mutable Dictionary

func removeObject(forKey: Any)

Removes a given key and its associated value from the dictionary.

func removeAllObjects()

Empties the dictionary of its entries.

