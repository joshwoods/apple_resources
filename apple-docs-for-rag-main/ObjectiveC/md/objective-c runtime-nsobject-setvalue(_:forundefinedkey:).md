

- Objective-C Runtime
- NSObject
-  setValue(\_:forUndefinedKey:) 

Instance Method

# setValue(\_:forUndefinedKey:)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setValue(
    _ value: Any?,
    forUndefinedKey key: String
)
```

## Parameters 

`value`  

The value for the key identified by `key`.

`key`  

A string that is not equal to the name of any of the receiver’s properties.

## Discussion

Subclasses can override this method to handle the request in some other way. The default implementation raises an `NSUndefinedKeyException`.

## See Also

### Related Documentation

func value(forUndefinedKey: String) -> Any?

Invoked by value(forKey:) when it finds no property corresponding to a given key.

### Setting Values

func setValue(Any?, forKeyPath: String)

Sets the value for the property identified by a given key path to a given value.

func setValuesForKeys([String : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

func setNilValueForKey(String)

Invoked by setValue(_:forKey:) when it’s given a `nil` value for a scalar value (such as an `int` or `float`).

func setValue(Any?, forKey: String)

Sets the property of the receiver specified by a given key to a given value.

