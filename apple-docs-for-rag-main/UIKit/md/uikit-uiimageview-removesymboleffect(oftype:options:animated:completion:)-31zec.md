

- UIKit
- UIImageView
-  removeSymbolEffect(ofType:options:animated:completion:) 

Instance Method

# removeSymbolEffect(ofType:options:animated:completion:)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
func removeSymbolEffect(
    ofType effect: some DiscreteSymbolEffect & IndefiniteSymbolEffect & SymbolEffect,
    options: SymbolEffectOptions = .default,
    animated: Bool = true,
    completion: UISymbolEffectCompletion? = nil
)
```

## Parameters 

`effect`  

The symbol effect to match for removal.

`options`  

The options to use when removing the symbol effect.

`animated`  

A Boolean value that indicates whether to animate the removal of a scale, appear, or disappear effect.

`completion`  

A completion handler the system calls after the removal is complete.

## See Also

### Configuring symbol effects

func addSymbolEffect(some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Adds a discrete symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Adds a discrete, indefinite symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Adds an indefinite symbol effect to the image view with the specified options and animation.

func setSymbolImage(UIImage, contentTransition: some ContentTransitionSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, completion: UISymbolEffectCompletion?)

Sets a symbol image using the specified content-transition effect, options, and completion handler.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the image view, using the specified options and animation setting.

typealias UISymbolEffectCompletion

A completion handler for adding and removing symbol effects and transitions.

struct UISymbolEffectCompletionContext

Information about a symbol effect’s addition or removal.

