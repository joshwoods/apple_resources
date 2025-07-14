

- Objective-C Runtime
- NSObject
-  value(forKeyPath:) 

Instance Method

# value(forKeyPath:)

Returns the value for the derived property identified by a given key path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func value(forKeyPath keyPath: String) -> Any?
```

## Parameters 

`keyPath`  

A key path of the form relationship.property (with one or more relationships); for example “department.name” or “department.manager.lastName”.

## Return Value

The value for the derived property identified by `keyPath`.

## Discussion

The default implementation gets the destination object for each relationship using value(forKey:) and returns the result of a value(forKey:) message to the final object.

## See Also

### Related Documentation

func setValue(Any?, forKeyPath: String)

Sets the value for the property identified by a given key path to a given value.

### Getting Values

func value(forKey: String) -> Any?

Returns the value for the property identified by a given key.

func dictionaryWithValues(forKeys: [String]) -> [String : Any]

Returns a dictionary containing the property values identified by each of the keys in a given array.

func value(forUndefinedKey: String) -> Any?

Invoked by value(forKey:) when it finds no property corresponding to a given key.

func mutableArrayValue(forKey: String) -> NSMutableArray

Returns a mutable array proxy that provides read-write access to an ordered to-many relationship specified by a given key.

func mutableArrayValue(forKeyPath: String) -> NSMutableArray

Returns a mutable array that provides read-write access to the ordered to-many relationship specified by a given key path.

func mutableSetValue(forKey: String) -> NSMutableSet

Returns a mutable set proxy that provides read-write access to the unordered to-many relationship specified by a given key.

func mutableSetValue(forKeyPath: String) -> NSMutableSet

Returns a mutable set that provides read-write access to the unordered to-many relationship specified by a given key path.

func mutableOrderedSetValue(forKey: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key.

func mutableOrderedSetValue(forKeyPath: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key path.

