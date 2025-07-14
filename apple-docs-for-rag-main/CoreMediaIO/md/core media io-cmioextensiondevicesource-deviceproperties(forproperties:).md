

- Core Media I/O
- CMIOExtensionDeviceSource
-  deviceProperties(forProperties:) 

Instance Method

# deviceProperties(forProperties:)

Retrieves the state of device properties.

Mac Catalyst 15.4+macOS 12.3+

``` source
func deviceProperties(forProperties properties: Set) throws -> CMIOExtensionDeviceProperties
```

**Required**

## Parameters 

`properties`  

A set of device properties to retrieve.

## Return Value

A properties object that contains the current device state.

## See Also

### Managing Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of available properties that a device provides.

**Required**

func setDeviceProperties(CMIOExtensionDeviceProperties) throws

Sets the state of device properties.

**Required**

