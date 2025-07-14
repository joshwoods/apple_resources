

- SpriteKit
- SKTextureAtlas
-  preloadTextureAtlases(\_:withCompletionHandler:) 

Type Method

# preloadTextureAtlases(\_:withCompletionHandler:)

Loads the textures of multiple atlas objects into memory, calling a completion handler after the task completes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func preloadTextureAtlases(
    _ textureAtlases: [SKTextureAtlas],
    withCompletionHandler completionHandler: @escaping () -> Void
)
```

``` source
class func preloadTextureAtlases(_ textureAtlases: [SKTextureAtlas]) async
```

## Parameters 

`textureAtlases`  

An array of SKTextureAtlas objects.

`completionHandler`  

A block called after all of the texture atlases are loaded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func preloadTextureAtlases(_ textureAtlases: [SKTextureAtlas]) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

SpriteKit creates a background task that loads the texture data from all of the specified atlas objects. Then, SpriteKit returns control to your game. After the atlas objects are loaded, your completion handler is called.

## See Also

### Preloading Textures

func preload(completionHandler: () -> Void)

Loads an atlas object’s textures into memory, calling a completion handler after the task completes.

class func preloadTextureAtlasesNamed([String], withCompletionHandler: ((any Error)?, [SKTextureAtlas]) -> Void)

Loads the textures of multiple atlases into memory, calling a completion handler after the task completes.

