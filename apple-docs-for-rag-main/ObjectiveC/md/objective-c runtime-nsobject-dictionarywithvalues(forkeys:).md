

- Objective-C Runtime
- NSObject
-  dictionaryWithValues(forKeys:) 

Instance Method

# dictionaryWithValues(forKeys:)

Returns a dictionary containing the property values identified by each of the keys in a given array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func dictionaryWithValues(forKeys keys: [String]) -> [String : Any]
```

## Parameters 

`keys`  

An array containing `NSString` objects that identify properties of the receiver.

## Return Value

A dictionary containing as keys the property names in `keys`, with corresponding values being the corresponding property values.

## Discussion

The default implementation invokes value(forKey:) for each key in `keys` and substitutes `NSNull` values in the dictionary for returned `nil` values.

## See Also

### Related Documentation

func setValuesForKeys([String : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

### Getting Values

func value(forKey: String) -> Any?

Returns the value for the property identified by a given key.

func value(forKeyPath: String) -> Any?

Returns the value for the derived property identified by a given key path.

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

