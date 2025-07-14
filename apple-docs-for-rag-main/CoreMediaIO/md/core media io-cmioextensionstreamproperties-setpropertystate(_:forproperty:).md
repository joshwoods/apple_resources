

- Core Media I/O
- CMIOExtensionStreamProperties
-  setPropertyState(\_:forProperty:) 

Instance Method

# setPropertyState(\_:forProperty:)

Sets the state of the specified property.

Mac Catalyst 15.4+macOS 12.3+

``` source
func setPropertyState(
    _ propertyState: CMIOExtensionPropertyState?,
    forProperty property: CMIOExtensionProperty
)
```

## Parameters 

`propertyState`  

The new state for the property.

`property`  

The property to update.

## See Also

### Managing Property State

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary representation of the property state.

