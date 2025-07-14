

- Foundation
- NSMutableDictionary
-  setObject(\_:forKey:) 

Instance Method

# setObject(\_:forKey:)

Adds a given key-value pair to the dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setObject(
    _ anObject: Any,
    forKey aKey: any NSCopying
)
```

## Parameters 

`anObject`  

The value for `aKey`. A strong reference to the object is maintained by the dictionary.

Important

Raises an invalidArgumentException if `anObject` is `nil`. If you need to represent a `nil` value in the dictionary, use NSNull.

`aKey`  

The key for `value`. The key is copied (using copy(with:); keys must conform to the `NSCopying` protocol). If `aKey` already exists in the dictionary, `anObject` takes its place.

Important

Raises an invalidArgumentException if `aKey` is `nil`.

## See Also

### Related Documentation

func removeObject(forKey: Any)

Removes a given key and its associated value from the dictionary.

### Adding Entries to a Mutable Dictionary

func setValue(Any?, forKey: String)

Adds a given key-value pair to the dictionary.

func addEntries(from: [AnyHashable : Any])

Adds to the receiving dictionary the entries from another dictionary.

func setDictionary([AnyHashable : Any])

Sets the contents of the receiving dictionary to entries in a given dictionary.

