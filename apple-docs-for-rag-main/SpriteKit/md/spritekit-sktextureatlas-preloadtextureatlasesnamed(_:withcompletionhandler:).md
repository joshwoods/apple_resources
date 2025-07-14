

- SpriteKit
- SKTextureAtlas
-  preloadTextureAtlasesNamed(\_:withCompletionHandler:) 

Type Method

# preloadTextureAtlasesNamed(\_:withCompletionHandler:)

Loads the textures of multiple atlases into memory, calling a completion handler after the task completes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func preloadTextureAtlasesNamed(
    _ atlasNames: [String],
    withCompletionHandler completionHandler: @escaping ((any Error)?, [SKTextureAtlas]) -> Void
)
```

``` source
class func preloadTextureAtlasesNamed(_ atlasNames: [String]) async throws -> [SKTextureAtlas]
```

## Parameters 

`atlasNames`  

An array containing the atlas names to preload.

`completionHandler`  

A block called after all of the texture atlases are loaded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func preloadTextureAtlasesNamed(_ atlasNames: [String]) async throws -> [SKTextureAtlas]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

SpriteKit creates a background task that loads the texture data from all of the specified atlas objects. Then, SpriteKit returns control to your game. After the atlases are loaded, your completion handler is called.

## See Also

### Preloading Textures

func preload(completionHandler: () -> Void)

Loads an atlas object’s textures into memory, calling a completion handler after the task completes.

class func preloadTextureAtlases([SKTextureAtlas], withCompletionHandler: () -> Void)

Loads the textures of multiple atlas objects into memory, calling a completion handler after the task completes.

