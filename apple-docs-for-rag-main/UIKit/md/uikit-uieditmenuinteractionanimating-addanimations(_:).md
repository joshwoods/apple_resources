

- UIKit
- UIEditMenuInteractionAnimating
-  addAnimations(\_:) 

Instance Method

# addAnimations(\_:)

Adds a closure that performs animations to run alongside the edit menu interaction presentation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func addAnimations(_ animations: @escaping () -> Void)
```

**Required**

## Parameters 

`animations`  

A closure that performs animations.

## See Also

### Adding Animations

func addCompletion(() -> Void)

Adds a closure to perform operations when the edit menu interaction presentation animations are complete.

**Required**

