

- SceneKit
- SCNScene
-  setAttribute(\_:forKey:) 

Instance Method

# setAttribute(\_:forKey:)

Sets a scene attribute for the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setAttribute(
    _ attribute: Any?,
    forKey key: String
)
```

## Parameters 

`attribute`  

An object that specifies the value of the attribute to be written.

`key`  

One of the constants described in Scene Attributes that identifies the attribute to be written.

## See Also

### Managing Scene Attributes

func attribute(forKey: String) -> Any?

Returns the scene attribute for the specified key.

struct Attribute

