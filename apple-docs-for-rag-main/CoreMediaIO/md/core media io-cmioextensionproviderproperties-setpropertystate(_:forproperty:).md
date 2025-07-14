

- Core Media I/O
- CMIOExtensionProviderProperties
-  setPropertyState(\_:forProperty:) 

Instance Method

# setPropertyState(\_:forProperty:)

Sets a state value for the specified property.

Mac Catalyst 15.4+macOS 12.3+

``` source
func setPropertyState(
    _ propertyState: CMIOExtensionPropertyState?,
    forProperty property: CMIOExtensionProperty
)
```

## Parameters 

`propertyState`  

The updated property state.

`property`  

The property to update.

## Discussion

Setting a `nil` property state value doesn’t remove the property.

## See Also

### Managing Properties

var name: String?

The provider name.

var manufacturer: String?

The provider manufacturer.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a provider.

