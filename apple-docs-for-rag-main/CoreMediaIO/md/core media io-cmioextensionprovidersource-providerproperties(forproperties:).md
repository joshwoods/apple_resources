

- Core Media I/O
- CMIOExtensionProviderSource
-  providerProperties(forProperties:) 

Instance Method

# providerProperties(forProperties:)

Gets the state of provider properties.

Mac Catalyst 15.4+macOS 12.3+

``` source
func providerProperties(forProperties properties: Set) throws -> CMIOExtensionProviderProperties
```

**Required**

## Parameters 

`properties`  

A set of properties for which to retrieve the state.

## Return Value

A provider properties object that contains the state of the requested properties.

## See Also

### Configuring Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of available properties for a provider.

**Required**

func setProviderProperties(CMIOExtensionProviderProperties) throws

Set the state of provider properties.

**Required**

