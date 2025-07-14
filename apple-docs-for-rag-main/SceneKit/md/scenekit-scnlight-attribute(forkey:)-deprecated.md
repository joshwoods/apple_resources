

- SceneKit
- SCNLight
-  attribute(forKey:) Deprecated

Instance Method

# attribute(forKey:)

Returns the value of a lighting attribute.

macOS 10.8–10.10Deprecated

``` source
func attribute(forKey key: String) -> Any?
```

Deprecated

Use properties instead. The property corresponding to each deprecated attribute is listed in Lighting Attribute Keys.

## Parameters 

`key`  

A constant specifying a lighting attribute. See Lighting Attribute Keys for available keys and their possible values.

## Return Value

The value of the lighting attribute, or `nil` if no such attribute exists.

## Discussion

A light’s type property determines its set of available attributes.

You can also get the values of lighting attributes using Key-value coding. The key path for each lighting attribute is listed in Lighting Attribute Keys.

## See Also

### Managing Light Attributes

var name: String?

A name associated with the light.

func setAttribute(Any?, forKey: String)

Sets the value for a lighting attribute.

Deprecated

Lighting Attribute Keys

Keys for specifying the behavior of a light using the attribute(forKey:) and setAttribute(_:forKey:) methods.

