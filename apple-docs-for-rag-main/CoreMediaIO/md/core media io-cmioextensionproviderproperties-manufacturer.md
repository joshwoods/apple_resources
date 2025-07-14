

- Core Media I/O
- CMIOExtensionProviderProperties
-  manufacturer 

Instance Property

# manufacturer

The provider manufacturer.

Mac Catalyst 15.4+macOS 12.3+

``` source
var manufacturer: String? { get set }
```

## Discussion

The key for this property is providerManufacturer.

## See Also

### Managing Properties

var name: String?

The provider name.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets a state value for the specified property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a provider.

