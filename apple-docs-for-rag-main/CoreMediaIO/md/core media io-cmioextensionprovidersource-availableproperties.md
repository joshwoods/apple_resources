

- Core Media I/O
- CMIOExtensionProviderSource
-  availableProperties 

Instance Property

# availableProperties

A set of available properties for a provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
var availableProperties: Set { get }
```

**Required**

## Discussion

Don’t change this property value during the life cycle of the associated provider.

## See Also

### Configuring Properties

func providerProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionProviderProperties

Gets the state of provider properties.

**Required**

func setProviderProperties(CMIOExtensionProviderProperties) throws

Set the state of provider properties.

**Required**

