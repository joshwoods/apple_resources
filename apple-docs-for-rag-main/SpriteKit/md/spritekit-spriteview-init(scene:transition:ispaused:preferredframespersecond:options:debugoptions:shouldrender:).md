

- SpriteKit
- SpriteView
-  init(scene:transition:isPaused:preferredFramesPerSecond:options:debugOptions:shouldRender:) 

Initializer

# init(scene:transition:isPaused:preferredFramesPerSecond:options:debugOptions:shouldRender:)

SpriteKitSwiftUIiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS

``` source
@preconcurrency nonisolated
init(
    scene: SKScene,
    transition: SKTransition? = nil,
    isPaused: Bool = false,
    preferredFramesPerSecond: Int = 60,
    options: SpriteView.Options = [.shouldCullNonVisibleNodes],
    debugOptions: SpriteView.DebugOptions,
    shouldRender: @escaping @MainActor (TimeInterval) -> Bool = { _ in true }
)
```

## See Also

### Creating a Sprite View

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int)

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int, options: SpriteView.Options, shouldRender: (TimeInterval) -> Bool)

struct Options

struct DebugOptions

