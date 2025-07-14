

- Objective-C Runtime
- NSObject
-  setValue(\_:forKeyPath:) 

Instance Method

# setValue(\_:forKeyPath:)

Sets the value for the property identified by a given key path to a given value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setValue(
    _ value: Any?,
    forKeyPath keyPath: String
)
```

## Parameters 

`value`  

The value for the property identified by `keyPath`.

`keyPath`  

A key path of the form relationship.property (with one or more relationships): for example “department.name” or “department.manager.lastName.”

## Discussion

The default implementation of this method gets the destination object for each relationship using value(forKey:), and sends the final object a setValue(_:forKey:) message.

### Special Considerations

When using this method, and the destination object does not implement an accessor for the value, the default behavior is for that object to retain `value` rather than copy or assign `value`.

## See Also

### Related Documentation

func value(forKeyPath: String) -> Any?

Returns the value for the derived property identified by a given key path.

### Setting Values

func setValuesForKeys([String : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

func setNilValueForKey(String)

Invoked by setValue(_:forKey:) when it’s given a `nil` value for a scalar value (such as an `int` or `float`).

func setValue(Any?, forKey: String)

Sets the property of the receiver specified by a given key to a given value.

func setValue(Any?, forUndefinedKey: String)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

