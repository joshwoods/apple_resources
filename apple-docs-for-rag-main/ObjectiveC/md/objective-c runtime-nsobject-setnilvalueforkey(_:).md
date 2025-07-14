

- Objective-C Runtime
- NSObject
-  setNilValueForKey(\_:) 

Instance Method

# setNilValueForKey(\_:)

Invoked by setValue(_:forKey:) when it’s given a `nil` value for a scalar value (such as an `int` or `float`).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setNilValueForKey(_ key: String)
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Discussion

Subclasses can override this method to handle the request in some other way, such as by substituting `0` or a sentinel value for `nil` and invoking setValue(_:forKey:) again or setting the variable directly. The default implementation raises an `NSInvalidArgumentException`.

## See Also

### Setting Values

func setValue(Any?, forKeyPath: String)

Sets the value for the property identified by a given key path to a given value.

func setValuesForKeys([String : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

func setValue(Any?, forKey: String)

Sets the property of the receiver specified by a given key to a given value.

func setValue(Any?, forUndefinedKey: String)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

