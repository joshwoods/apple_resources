

- AppKit
- NSImageView
-  addSymbolEffect(\_:options:animated:) 

Instance Method

# addSymbolEffect(\_:options:animated:)

Adds a discrete, indefinite symbol effect to the image view with the specified options and animation.

macOS 14.0+

``` source
@MainActor @preconcurrency
func addSymbolEffect(
    _ effect: some DiscreteSymbolEffect & IndefiniteSymbolEffect & SymbolEffect,
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

func addSymbolEffect(some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds an indefinite symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete symbol effect to the image view with the specified options and animation.

func setSymbolImage(NSImage, contentTransition: some ContentTransitionSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions)

Sets a symbol image using the specified content-transition effect and options.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the image view, using the specified options and animation setting.

