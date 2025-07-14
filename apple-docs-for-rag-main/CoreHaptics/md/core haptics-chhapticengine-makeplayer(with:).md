

- Core Haptics
- CHHapticEngine
-  makePlayer(with:) 

Instance Method

# makePlayer(with:)

Creates a standard haptic pattern player from a haptic pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func makePlayer(with pattern: CHHapticPattern) throws -> any CHHapticPatternPlayer
```

## Parameters 

`pattern`  

The haptic pattern you’d like the player to play.

## Return Value

A new pattern player instance.

## Mentioned in 

Playing a single-tap haptic pattern

Preparing your app to play haptics

## See Also

### Creating Haptic Pattern Players

func makeAdvancedPlayer(with: CHHapticPattern) throws -> any CHHapticAdvancedPatternPlayer

Creates an advanced haptic pattern player from a haptic pattern.

