

- Foundation
- NSMutableDictionary
-  removeObject(forKey:) 

Instance Method

# removeObject(forKey:)

Removes a given key and its associated value from the dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObject(forKey aKey: Any)
```

## Parameters 

`aKey`  

The key to remove.

Important

Raises an invalidArgumentException if `aKey` is `nil`.

## Discussion

Does nothing if `aKey` does not exist.

For example, assume you have an archived dictionary that records the call letters and associated frequencies of radio stations. To remove an entry for a defunct station, you could write code similar to the following:

```
NSMutableDictionary *stations = nil;

stations = [[NSMutableDictionary alloc]
        initWithContentsOfFile: pathToArchive];
[stations removeObjectForKey:@"KIKT"];
```

## See Also

### Removing Entries From a Mutable Dictionary

func removeAllObjects()

Empties the dictionary of its entries.

func removeObjects(forKeys: [Any])

Removes from the dictionary entries specified by elements in a given array.

