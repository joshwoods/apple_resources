

- Foundation
- NSMutableDictionary
-  setDictionary(\_:) 

Instance Method

# setDictionary(\_:)

Sets the contents of the receiving dictionary to entries in a given dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setDictionary(_ otherDictionary: [AnyHashable : Any])
```

## Parameters 

`otherDictionary`  

A dictionary containing the new entries.

## Discussion

All entries are removed from the receiving dictionary (with removeAllObjects()), then each entry from `otherDictionary` added into the receiving dictionary.

## See Also

### Adding Entries to a Mutable Dictionary

func setObject(Any, forKey: any NSCopying)

Adds a given key-value pair to the dictionary.

func setValue(Any?, forKey: String)

Adds a given key-value pair to the dictionary.

func addEntries(from: [AnyHashable : Any])

Adds to the receiving dictionary the entries from another dictionary.

