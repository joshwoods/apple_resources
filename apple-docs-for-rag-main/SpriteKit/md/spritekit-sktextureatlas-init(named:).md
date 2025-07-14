

- SpriteKit
- SKTextureAtlas
-  init(named:) 

Initializer

# init(named:)

Creates a texture atlas from data stored in the app bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(named name: String)
```

## Parameters 

`name`  

The name of the texture atlas, without the `.atlas` extension.

## Return Value

A new texture atlas object.

## Discussion

If the texture atlas cannot be found, an exception is thrown.

## See Also

### Creating a Texture Atlas Programmatically

convenience init(dictionary: [String : Any])

Creates a texture atlas from a set of image files.

