

- Objective-C Runtime
- NSObject
-  validateValue(\_:forKey:) 

Instance Method

# validateValue(\_:forKey:)

Indicates whether the value specified by a given pointer is valid, or can be made valid, for the property identified by a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func validateValue(
    _ ioValue: AutoreleasingUnsafeMutablePointer,
    forKey inKey: String
) throws
```

## Parameters 

`ioValue`  

A pointer to a new value for the property identified by `inKey`. This method may modify or replace the value in order to make it valid.

`inKey`  

The name of one of the receiver’s properties. The key must specify an attribute or a to-one relationship.

## Discussion

In Swift, this method throws an error if the value isn’t valid. In Objective-C, it returns a Boolean value.

The default implementation of this function searches the class of the receiver for a property-specific validation function with a particular signature, allowing that function to determine the outcome of the validation. For it to be found, the property-specific validation function must be exposed to Objective-C, must be named according to the pattern `validate`, must take a single, optional `AnyObject` pointer argument, and must throw. For example, for a property named `someString`, the validation function is:

```
```

If you define such a function, the default implementation of validateValue(_:forKey:) calls it when asked to validate the corresponding property, allowing your function to either alter the input value or throw an error.

If no such function exists for a particular property, validateValue(_:forKey:)returns YES without taking any other action. In other words, by default, the general validation call succeeds if you don’t explicitly provide a validation function for the given property.

Note

You typically use the validation described here only in Objective-C. In Swift, property validation is more idiomatically handled by relying on compiler support for optionals and strong type checking, while using the built-in `willSet` and `didSet` property observers to test any run-time API contracts, as described in the Property Observers section of The Swift Programming Language (Swift 4.1).

See Adding Validation in Key-Value Coding Programming Guide for more information.

## See Also

### Validation

func validateValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKeyPath: String) throws

Indicates whether the value specified by a given pointer is not valid for a given key path relative to the receiver.

