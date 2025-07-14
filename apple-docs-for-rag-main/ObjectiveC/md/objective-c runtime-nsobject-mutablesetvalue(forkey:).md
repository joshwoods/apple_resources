

- Objective-C Runtime
- NSObject
-  mutableSetValue(forKey:) 

Instance Method

# mutableSetValue(forKey:)

Returns a mutable set proxy that provides read-write access to the unordered to-many relationship specified by a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func mutableSetValue(forKey key: String) -> NSMutableSet
```

## Parameters 

`key`  

The name of an unordered to-many relationship.

## Return Value

A mutable set that provides read-write access to the unordered to-many relationship specified by `key`.

## Discussion

Objects added to the mutable set proxy become related to the receiver, and objects removed from the mutable set become unrelated. The default implementation recognizes the same simple accessor methods and set accessor methods as value(forKey:), and follows the same direct instance variable access policies, but always returns a mutable collection proxy object instead of the immutable collection that value(forKey:) would return.

The search pattern that `mutableSetValueForKey:` uses is described in Accessor Search Patterns in Key-Value Coding Programming Guide.

## See Also

### Getting Values

func value(forKey: String) -> Any?

Returns the value for the property identified by a given key.

func value(forKeyPath: String) -> Any?

Returns the value for the derived property identified by a given key path.

func dictionaryWithValues(forKeys: [String]) -> [String : Any]

Returns a dictionary containing the property values identified by each of the keys in a given array.

func value(forUndefinedKey: String) -> Any?

Invoked by value(forKey:) when it finds no property corresponding to a given key.

func mutableArrayValue(forKey: String) -> NSMutableArray

Returns a mutable array proxy that provides read-write access to an ordered to-many relationship specified by a given key.

func mutableArrayValue(forKeyPath: String) -> NSMutableArray

Returns a mutable array that provides read-write access to the ordered to-many relationship specified by a given key path.

func mutableSetValue(forKeyPath: String) -> NSMutableSet

Returns a mutable set that provides read-write access to the unordered to-many relationship specified by a given key path.

func mutableOrderedSetValue(forKey: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key.

func mutableOrderedSetValue(forKeyPath: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key path.

