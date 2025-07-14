

- Objective-C Runtime
- NSObject
-  validateValue(\_:forKeyPath:) 

Instance Method

# validateValue(\_:forKeyPath:)

Indicates whether the value specified by a given pointer is not valid for a given key path relative to the receiver.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func validateValue(
    _ ioValue: AutoreleasingUnsafeMutablePointer,
    forKeyPath inKeyPath: String
) throws
```

## Parameters 

`ioValue`  

A pointer to a new value for the property identified by `inKeyPath`. This method may modify or replace the value in order to make it valid.

`inKeyPath`  

The name of one of the receiver’s properties. The key path must specify an attribute or a to-one relationship. The key path has the form ``` relationship``.``property ``` (with one or more relationships); for example `department.name` or `department.manager.lastName`.

## Discussion

In Swift, this method throws an error if the value isn’t valid. In Objective-C, it returns a Boolean value.

The default implementation of this method gets the destination object for each relationship using value(forKey:) and returns the result of calling the validateValue(_:forKey:) method for the property.

## See Also

### Validation

func validateValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: String) throws

Indicates whether the value specified by a given pointer is valid, or can be made valid, for the property identified by a given key.

