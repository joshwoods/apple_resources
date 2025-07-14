

- UIKit
- UIImageView
-  setSymbolImage(\_:contentTransition:options:completion:) 

Instance Method

# setSymbolImage(\_:contentTransition:options:completion:)

Sets a symbol image using the specified content-transition effect, options, and completion handler.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
func setSymbolImage(
    _ image: UIImage,
    contentTransition: some ContentTransitionSymbolEffect & SymbolEffect,
    options: SymbolEffectOptions = .default,
    completion: UISymbolEffectCompletion? = nil
)
```

## Parameters 

`image`  

The symbol image to set.

`contentTransition`  

The content transition to use when setting the symbol image.

`options`  

The options to use when setting the symbol image.

`completion`  

A completion handler the system calls after setting the symbol image.

## See Also

### Configuring symbol effects

func addSymbolEffect(some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Adds a discrete symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Adds a discrete, indefinite symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Adds an indefinite symbol effect to the image view with the specified options and animation.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool, completion: UISymbolEffectCompletion?)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the image view, using the specified options and animation setting.

typealias UISymbolEffectCompletion

A completion handler for adding and removing symbol effects and transitions.

struct UISymbolEffectCompletionContext

Information about a symbol effect’s addition or removal.

