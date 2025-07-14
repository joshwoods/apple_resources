

- Objective-C Runtime
- NSObject
-  setValue(\_:forKey:) 

Instance Method

# setValue(\_:forKey:)

Sets the property of the receiver specified by a given key to a given value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setValue(
    _ value: Any?,
    forKey key: String
)
```

## Parameters 

`value`  

The value for the property identified by `key`.

`key`  

The name of one of the receiver’s properties.

## Discussion

If `key` identifies a to-one relationship, relate the object specified by `value` to the receiver, unrelating the previously related object if there was one. Given a collection object and a `key` that identifies a to-many relationship, relate the objects contained in the collection to the receiver, unrelating previously related objects if there were any.

The search pattern that `setValue:forKey:` uses is described in Accessor Search Patterns in Key-Value Coding Programming Guide.

In a reference-counted environment, if the instance variable is accessed directly, `value` is retained.

## See Also

### Setting Values

func setValue(Any?, forKeyPath: String)

Sets the value for the property identified by a given key path to a given value.

func setValuesForKeys([String : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

func setNilValueForKey(String)

Invoked by setValue(_:forKey:) when it’s given a `nil` value for a scalar value (such as an `int` or `float`).

func setValue(Any?, forUndefinedKey: String)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

