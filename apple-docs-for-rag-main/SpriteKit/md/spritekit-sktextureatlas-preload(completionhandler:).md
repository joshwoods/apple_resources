

- SpriteKit
- SKTextureAtlas
-  preload(completionHandler:) 

Instance Method

# preload(completionHandler:)

Loads an atlas object’s textures into memory, calling a completion handler after the task completes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func preload(completionHandler: @escaping () -> Void)
```

``` source
func preload() async
```

## Parameters 

`completionHandler`  

A block called after the texture atlas is loaded.

## Mentioned in 

Maximizing Texture Performance

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func preload() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

SpriteKit creates a background task that loads the texture data from the atlas object. Then, SpriteKit returns control to your game. After the texture atlas is loaded, your completion handler is called.

If you need to preload multiple texture atlas objects immediately, use the preloadTextureAtlases(_:withCompletionHandler:) method instead.

## See Also

### Preloading Textures

class func preloadTextureAtlases([SKTextureAtlas], withCompletionHandler: () -> Void)

Loads the textures of multiple atlas objects into memory, calling a completion handler after the task completes.

class func preloadTextureAtlasesNamed([String], withCompletionHandler: ((any Error)?, [SKTextureAtlas]) -> Void)

Loads the textures of multiple atlases into memory, calling a completion handler after the task completes.

