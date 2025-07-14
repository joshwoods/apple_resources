

- Core Media I/O
- CMIOExtensionDeviceSource
-  setDeviceProperties(\_:) 

Instance Method

# setDeviceProperties(\_:)

Sets the state of device properties.

Mac Catalyst 15.4+macOS 12.3+

``` source
func setDeviceProperties(_ deviceProperties: CMIOExtensionDeviceProperties) throws
```

**Required**

## Parameters 

`deviceProperties`  

A properties object that contains the updated device state.

## Discussion

If you implement this method in Swift and an error occurs, throw an error and pass more detailed information regarding the property or properties that failed in the error that you throw. If you implement this method in Objective-C and an error occurs, pass more detailed information regarding the property or properties that failed in the localizedDescription property of NSError.

Note

The property attributes associated with a property state are always `nil` when setting a value.

## See Also

### Managing Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of available properties that a device provides.

**Required**

func deviceProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionDeviceProperties

Retrieves the state of device properties.

**Required**

