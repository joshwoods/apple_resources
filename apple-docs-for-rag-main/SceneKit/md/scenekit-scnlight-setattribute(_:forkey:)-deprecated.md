

- SceneKit
- SCNLight
-  setAttribute(\_:forKey:) Deprecated

Instance Method

# setAttribute(\_:forKey:)

Sets the value for a lighting attribute.

macOS 10.8–10.10Deprecated

``` source
func setAttribute(
    _ attribute: Any?,
    forKey key: String
)
```

Deprecated

Use properties instead. The property corresponding to each deprecated attribute is listed in Lighting Attribute Keys.

## Parameters 

`attribute`  

The value for the lighting attribute.

`key`  

A constant specifying a lighting attribute. See Lighting Attribute Keys for available keys and their possible values.

## Discussion

A light’s type property determines its set of available attributes.

You can also set or animate changes to the values of lighting attributes using Key-value coding. The key path for each lighting attribute is listed in Lighting Attribute Keys.

## See Also

### Managing Light Attributes

var name: String?

A name associated with the light.

func attribute(forKey: String) -> Any?

Returns the value of a lighting attribute.

Deprecated

Lighting Attribute Keys

Keys for specifying the behavior of a light using the attribute(forKey:) and setAttribute(_:forKey:) methods.

