

- UIKit
- UIEditMenuInteractionAnimating
-  addCompletion(\_:) 

Instance Method

# addCompletion(\_:)

Adds a closure to perform operations when the edit menu interaction presentation animations are complete.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func addCompletion(_ completion: @escaping () -> Void)
```

**Required**

## Parameters 

`completion`  

A closure that performs operations after the animations complete.

## See Also

### Adding Animations

func addAnimations(() -> Void)

Adds a closure that performs animations to run alongside the edit menu interaction presentation.

**Required**

