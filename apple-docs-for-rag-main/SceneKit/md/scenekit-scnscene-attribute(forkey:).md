

- SceneKit
- SCNScene
-  attribute(forKey:) 

Instance Method

# attribute(forKey:)

Returns the scene attribute for the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func attribute(forKey key: String) -> Any?
```

## Parameters 

`key`  

One of the constants described in Scene Attributes that identifies the attribute to be read.

## Return Value

The scene attribute for the specified key, or `nil` if no such attribute exists.

## See Also

### Managing Scene Attributes

func setAttribute(Any?, forKey: String)

Sets a scene attribute for the specified key.

struct Attribute

