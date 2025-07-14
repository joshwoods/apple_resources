

- Foundation
- NSMutableDictionary
-  addEntries(from:) 

Instance Method

# addEntries(from:)

Adds to the receiving dictionary the entries from another dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addEntries(from otherDictionary: [AnyHashable : Any])
```

## Parameters 

`otherDictionary`  

The dictionary from which to add entries

## Discussion

Each value object from `otherDictionary` is sent a retain message before being added to the receiving dictionary. In contrast, each key object is copied (using copy(with:)—keys must conform to the `NSCopying` protocol), and the copy is added to the receiving dictionary.

If both dictionaries contain the same key, the receiving dictionary’s previous value object for that key is sent a `release` message, and the new value object takes its place.

## See Also

### Adding Entries to a Mutable Dictionary

func setObject(Any, forKey: any NSCopying)

Adds a given key-value pair to the dictionary.

func setValue(Any?, forKey: String)

Adds a given key-value pair to the dictionary.

func setDictionary([AnyHashable : Any])

Sets the contents of the receiving dictionary to entries in a given dictionary.

