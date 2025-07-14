

- Core Media I/O
- CMIOExtensionProviderProperties
-  propertiesDictionary 

Instance Property

# propertiesDictionary

A dictionary of properties for a provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState] { get set }
```

## See Also

### Managing Properties

var name: String?

The provider name.

var manufacturer: String?

The provider manufacturer.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets a state value for the specified property.

