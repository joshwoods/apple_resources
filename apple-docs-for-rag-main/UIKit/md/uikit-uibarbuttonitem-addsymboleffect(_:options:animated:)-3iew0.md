

- UIKit
- UIBarButtonItem
-  addSymbolEffect(\_:options:animated:) 

Instance Method

# addSymbolEffect(\_:options:animated:)

Adds an indefinite symbol effect to the bar button item with the specified options and animation.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
func addSymbolEffect(
    _ effect: some IndefiniteSymbolEffect & SymbolEffect,
    options: SymbolEffectOptions = .default,
    animated: Bool = true
)
```

## Parameters 

`effect`  

The symbol effect to add.

`options`  

The options for the symbol effect.

`animated`  

A Boolean value that indicates whether to animate the addition of a scale, appear, or disappear effect.

## See Also

### Configuring symbol effects

var isSymbolAnimationEnabled: Bool

A Boolean value that indicates whether symbol effects animate.

func addSymbolEffect(some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete, indefinite symbol effect to the bar button item with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete symbol effect to the bar button item with the specified options and animation.

func setSymbolImage(UIImage, contentTransition: some ContentTransitionSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions)

Sets a symbol image using the specified content-transition effect and options.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the bar button item, using the specified options and animation setting.

