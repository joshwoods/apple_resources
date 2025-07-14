

- Model I/O
- MDLSkyCubeTexture
-  update() 

Instance Method

# update()

Generates new texel data matching the current sky parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func update()
```

## Discussion

After you first create a sky cube texture, Model I/O does not generate texture data until you use one of the MDLTexture methods listed inAccessing Texture Data. If you then change the sky simulation or rendering parameters, call this method to generate new texture data.

