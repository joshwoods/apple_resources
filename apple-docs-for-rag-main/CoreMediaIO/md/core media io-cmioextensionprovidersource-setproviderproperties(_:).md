

- Core Media I/O
- CMIOExtensionProviderSource
-  setProviderProperties(\_:) 

Instance Method

# setProviderProperties(\_:)

Set the state of provider properties.

Mac Catalyst 15.4+macOS 12.3+

``` source
func setProviderProperties(_ providerProperties: CMIOExtensionProviderProperties) throws
```

**Required**

## Parameters 

`providerProperties`  

A provider properties object that contains the updated property states.

## Discussion

If you implement this method in Swift and an error occurs, throw an error and pass more detailed information regarding the property or properties that failed in the error that you throw. If you implement this method in Objective-C and an error occurs, pass more detailed information regarding the property or properties that failed in the localizedDescription property of NSError.

## See Also

### Configuring Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of available properties for a provider.

**Required**

func providerProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionProviderProperties

Gets the state of provider properties.

**Required**

