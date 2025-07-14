

- SpriteKit
- SpriteView
-  SpriteView.DebugOptions 

Structure

# SpriteView.DebugOptions

SpriteKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct DebugOptions
```

## Topics

### Type Properties

static let showsDrawCount: SpriteView.DebugOptions

static let showsFPS: SpriteView.DebugOptions

static let showsFields: SpriteView.DebugOptions

static let showsNodeCount: SpriteView.DebugOptions

static let showsPhysics: SpriteView.DebugOptions

static let showsQuadCount: SpriteView.DebugOptions

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating a Sprite View

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int)

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int, options: SpriteView.Options, shouldRender: (TimeInterval) -> Bool)

init(scene: SKScene, transition: SKTransition?, isPaused: Bool, preferredFramesPerSecond: Int, options: SpriteView.Options, debugOptions: SpriteView.DebugOptions, shouldRender: (TimeInterval) -> Bool)

struct Options

