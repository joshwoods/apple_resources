

- SpriteKit
- SKTexture
-  preload(\_:withCompletionHandler:) 

Type Method

# preload(\_:withCompletionHandler:)

Load the data of multiple textures into memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func preload(
    _ textures: [SKTexture],
    withCompletionHandler completionHandler: @escaping () -> Void
)
```

``` source
class func preload(_ textures: [SKTexture]) async
```

## Parameters 

`textures`  

An array of SKTexture objects.

`completionHandler`  

A block called after all of the textures are loaded.

## Mentioned in 

Maximizing Texture Performance

Preloading Textures into Memory

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func preload(_ textures: [SKTexture]) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

SpriteKit creates a background task that loads the texture data for all of the textures in the array, then returns control to your game. Your completion handler is called after all of the textures are loaded.

## See Also

### Preloading a Texture for Performance

Preloading Textures into Memory

Decompress images ahead of time to avoid performance issues during gameplay.

func preload(completionHandler: () -> Void)

Load texture data into memory, calling a completion handler after the task completes.

