

- Core Haptics
- CHHapticEngine
-  makeAdvancedPlayer(with:) 

Instance Method

# makeAdvancedPlayer(with:)

Creates an advanced haptic pattern player from a haptic pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func makeAdvancedPlayer(with pattern: CHHapticPattern) throws -> any CHHapticAdvancedPatternPlayer
```

## Parameters 

`pattern`  

The haptic pattern you’d like the player to play.

## Return Value

A new advanced pattern player instance.

## See Also

### Creating Haptic Pattern Players

func makePlayer(with: CHHapticPattern) throws -> any CHHapticPatternPlayer

Creates a standard haptic pattern player from a haptic pattern.

