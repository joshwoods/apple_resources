

- Foundation
- NSMutableDictionary
-  removeAllObjects() 

Instance Method

# removeAllObjects()

Empties the dictionary of its entries.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeAllObjects()
```

## Discussion

Each key and corresponding value object is sent a release message.

## See Also

### Removing Entries From a Mutable Dictionary

func removeObject(forKey: Any)

Removes a given key and its associated value from the dictionary.

func removeObjects(forKeys: [Any])

Removes from the dictionary entries specified by elements in a given array.

