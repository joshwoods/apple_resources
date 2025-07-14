

- Objective-C Runtime
- NSObject
-  mutableArrayValue(forKeyPath:) 

Instance Method

# mutableArrayValue(forKeyPath:)

Returns a mutable array that provides read-write access to the ordered to-many relationship specified by a given key path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func mutableArrayValue(forKeyPath keyPath: String) -> NSMutableArray
```

## Parameters 

`keyPath`  

A key path, relative to the receiver, to an ordered to-many relationship.

## Return Value

A mutable array that provides read-write access to the ordered to-many relationship specified by `keyPath`.

## Discussion

See mutableArrayValue(forKey:) for additional details.

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

func mutableSetValue(forKey: String) -> NSMutableSet

Returns a mutable set proxy that provides read-write access to the unordered to-many relationship specified by a given key.

func mutableSetValue(forKeyPath: String) -> NSMutableSet

Returns a mutable set that provides read-write access to the unordered to-many relationship specified by a given key path.

func mutableOrderedSetValue(forKey: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key.

func mutableOrderedSetValue(forKeyPath: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key path.

