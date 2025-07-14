

- SpriteKit
-  SpriteView 

Structure

# SpriteView

A SwiftUI view that renders a SpriteKit scene.

SpriteKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@MainActor @preconcurrency
struct SpriteView
```

## Topics

### Creating a Sprite View

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int)

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int, options: SpriteView.Options, shouldRender: (TimeInterval) -> Bool)

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int, options: SpriteView.Options, debugOptions: SpriteView.DebugOptions, shouldRender: (TimeInterval) -> Bool)

struct Options

struct DebugOptions

## Relationships

### Conforms To

- Sendable
- View

