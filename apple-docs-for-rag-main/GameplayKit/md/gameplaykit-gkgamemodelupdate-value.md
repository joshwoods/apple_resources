

- GameplayKit
- GKGameModelUpdate
-  value 

Instance Property

# value

A value assigned and read by GameplayKit to rate the desirability of a move in your game.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var value: Int { get set }
```

**Required**

## Discussion

Your game does not assign to or read from this property directly. Instead, when you adopt the GKGameModelUpdate protocol, you simply provide a read/write implementation of this property. When you use the GKMinmaxStrategist class to select optimal moves during gameplay, GameplayKit assigns values to this property in order to rate the desirability of each move to a given player.

For more information, see GameplayKit Programming Guide.

