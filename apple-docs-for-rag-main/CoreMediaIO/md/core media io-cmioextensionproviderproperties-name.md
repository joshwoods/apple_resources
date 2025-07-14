

- Core Media I/O
- CMIOExtensionProviderProperties
-  name 

Instance Property

# name

The provider name.

Mac Catalyst 15.4+macOS 12.3+

``` source
var name: String? { get set }
```

## Discussion

The key for this property is providerName.

## See Also

### Managing Properties

var manufacturer: String?

The provider manufacturer.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets a state value for the specified property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a provider.

