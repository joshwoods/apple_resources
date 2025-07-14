

- Objective-C Runtime
- NSObject
-  setValuesForKeys(\_:) 

Instance Method

# setValuesForKeys(\_:)

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setValuesForKeys(_ keyedValues: [String : Any])
```

## Parameters 

`keyedValues`  

A dictionary whose keys identify properties in the receiver. The values of the properties in the receiver are set to the corresponding values in the dictionary.

## Discussion

The default implementation invokes setValue(_:forKey:) for each key-value pair, substituting `nil` for `NSNull` values in `keyedValues`.

## See Also

### Related Documentation

func dictionaryWithValues(forKeys: [String]) -> [String : Any]

Returns a dictionary containing the property values identified by each of the keys in a given array.

### Setting Values

func setValue(Any?, forKeyPath: String)

Sets the value for the property identified by a given key path to a given value.

func setNilValueForKey(String)

Invoked by setValue(_:forKey:) when it’s given a `nil` value for a scalar value (such as an `int` or `float`).

func setValue(Any?, forKey: String)

Sets the property of the receiver specified by a given key to a given value.

func setValue(Any?, forUndefinedKey: String)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

