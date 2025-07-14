

- Foundation
- NSMutableDictionary
-  setValue(\_:forKey:) 

Instance Method

# setValue(\_:forKey:)

Adds a given key-value pair to the dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setValue(
    _ value: Any?,
    forKey key: String
)
```

## Parameters 

`value`  

The value for `key`.

`key`  

The key for `value`. Note that when using key-value coding, the key must be a string (see Accessing Object Properties).

## Discussion

This method adds `value` and `key` to the dictionary using setObject(_:forKey:), unless `value` is `nil` in which case the method instead attempts to remove `key` using removeObject(forKey:).

## See Also

### Related Documentation

func value(forKey: String) -> Any?

Returns the value associated with a given key.

### Adding Entries to a Mutable Dictionary

func setObject(Any, forKey: any NSCopying)

Adds a given key-value pair to the dictionary.

func addEntries(from: [AnyHashable : Any])

Adds to the receiving dictionary the entries from another dictionary.

func setDictionary([AnyHashable : Any])

Sets the contents of the receiving dictionary to entries in a given dictionary.

