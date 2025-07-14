

- SpriteKit
- SKTexture
-  preload(completionHandler:) 

Instance Method

# preload(completionHandler:)

Load texture data into memory, calling a completion handler after the task completes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func preload(completionHandler: @escaping () -> Void)
```

``` source
func preload() async
```

## Parameters 

`completionHandler`  

A block called after the texture data is loaded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func preload() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

SpriteKit creates a background task to load the texture data from the associated file, then returns control to your game. After the texture data is loaded, your completion handler is called. Typically, you use this method when you want to guarantee that a particular texture is in memory before accessing it.

If you need to preload multiple textures at once, use the preload(_:withCompletionHandler:) method instead.

## See Also

### Preloading a Texture for Performance

Preloading Textures into Memory

Decompress images ahead of time to avoid performance issues during gameplay.

class func preload([SKTexture], withCompletionHandler: () -> Void)

Load the data of multiple textures into memory.

