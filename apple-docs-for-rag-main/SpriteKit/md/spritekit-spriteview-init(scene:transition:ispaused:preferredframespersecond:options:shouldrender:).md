

- SpriteKit
- SpriteView
-  init(scene:transition:isPaused:preferredFramesPerSecond:options:shouldRender:) 

Initializer

# init(scene:transition:isPaused:preferredFramesPerSecond:options:shouldRender:)

SpriteKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
@preconcurrency nonisolated
init(
    scene: SKScene,
    transition: SKTransition? = nil,
    isPaused: Bool = false,
    preferredFramesPerSecond: Int = 60,
    options: SpriteView.Options = [.shouldCullNonVisibleNodes],
    shouldRender: @escaping @MainActor (TimeInterval) -> Bool = { _ in true }
)
```

## See Also

### Creating a Sprite View

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int)

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int, options: SpriteView.Options, debugOptions: SpriteView.DebugOptions, shouldRender: (TimeInterval) -> Bool)

struct Options

struct DebugOptions

