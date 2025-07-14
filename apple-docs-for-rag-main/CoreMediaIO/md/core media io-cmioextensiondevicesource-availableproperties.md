

- Core Media I/O
- CMIOExtensionDeviceSource
-  availableProperties 

Instance Property

# availableProperties

A set of available properties that a device provides.

Mac Catalyst 15.4+macOS 12.3+

``` source
var availableProperties: Set { get }
```

**Required**

## Discussion

Don’t change the state of this property during the life cycle of the associated device.

## See Also

### Managing Properties

func deviceProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionDeviceProperties

Retrieves the state of device properties.

**Required**

func setDeviceProperties(CMIOExtensionDeviceProperties) throws

Sets the state of device properties.

**Required**

