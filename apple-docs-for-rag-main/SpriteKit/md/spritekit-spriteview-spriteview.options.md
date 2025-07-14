

- SpriteKit
- SpriteView
-  SpriteView.Options 

Structure

# SpriteView.Options

SpriteKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
struct Options
```

## Topics

### Type Properties

static let allowsTransparency: SpriteView.Options

static let ignoresSiblingOrder: SpriteView.Options

static let shouldCullNonVisibleNodes: SpriteView.Options

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

struct DebugOptions

