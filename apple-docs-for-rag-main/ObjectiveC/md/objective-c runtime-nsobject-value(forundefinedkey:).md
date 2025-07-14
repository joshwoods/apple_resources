

- Objective-C Runtime
- NSObject
-  value(forUndefinedKey:) 

Instance Method

# value(forUndefinedKey:)

Invoked by value(forKey:) when it finds no property corresponding to a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func value(forUndefinedKey key: String) -> Any?
```

## Parameters 

`key`  

A string that is not equal to the name of any of the receiver’s properties.

## Discussion

Subclasses can override this method to return an alternate value for undefined keys. The default implementation raises an `NSUndefinedKeyException`.

## See Also

### Related Documentation

func setValue(Any?, forUndefinedKey: String)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

### Getting Values

func value(forKey: String) -> Any?

Returns the value for the property identified by a given key.

func value(forKeyPath: String) -> Any?

Returns the value for the derived property identified by a given key path.

func dictionaryWithValues(forKeys: [String]) -> [String : Any]

Returns a dictionary containing the property values identified by each of the keys in a given array.

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

