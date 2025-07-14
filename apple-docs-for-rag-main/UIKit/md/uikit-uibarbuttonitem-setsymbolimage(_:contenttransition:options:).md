

- UIKit
- UIBarButtonItem
-  setSymbolImage(\_:contentTransition:options:) 

Instance Method

# setSymbolImage(\_:contentTransition:options:)

Sets a symbol image using the specified content-transition effect and options.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
func setSymbolImage(
    _ image: UIImage,
    contentTransition: some ContentTransitionSymbolEffect & SymbolEffect,
    options: SymbolEffectOptions = .default
)
```

## Parameters 

`image`  

The symbol image to set.

`contentTransition`  

The content transition to use when setting the symbol image.

`options`  

The options to use when setting the symbol image.

## See Also

### Configuring symbol effects

var isSymbolAnimationEnabled: Bool

A Boolean value that indicates whether symbol effects animate.

func addSymbolEffect(some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds an indefinite symbol effect to the bar button item with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete, indefinite symbol effect to the bar button item with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete symbol effect to the bar button item with the specified options and animation.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the bar button item, using the specified options and animation setting.

