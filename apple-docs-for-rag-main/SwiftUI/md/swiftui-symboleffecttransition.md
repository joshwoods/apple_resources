

- SwiftUI
-  SymbolEffectTransition 

Structure

# SymbolEffectTransition

Creates a transition that applies the Appear or Disappear symbol animation to symbol images within the inserted or removed view hierarchy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @frozen @preconcurrency
struct SymbolEffectTransition
```

## Overview

Other views are unaffected by this transition.

## Topics

### Creating a transition

init&lt;T>(effect: T, options: SymbolEffectOptions)

## Relationships

### Conforms To

- Transition

## See Also

### Managing symbol effects

func symbolEffect&lt;T>(T, options: SymbolEffectOptions, isActive: Bool) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffect&lt;T, U>(T, options: SymbolEffectOptions, value: U) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffectsRemoved(Bool) -> some View

Returns a new view with its inherited symbol image effects either removed or left unchanged.

