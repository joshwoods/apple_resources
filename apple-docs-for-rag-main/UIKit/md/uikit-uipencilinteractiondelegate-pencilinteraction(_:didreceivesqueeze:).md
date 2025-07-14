

- UIKit
- UIPencilInteractionDelegate
-  pencilInteraction(\_:didReceiveSqueeze:) 

Instance Method

# pencilInteraction(\_:didReceiveSqueeze:)

Tells the delegate when a person squeezes Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
optional func pencilInteraction(
    _ interaction: UIPencilInteraction,
    didReceiveSqueeze squeeze: UIPencilInteraction.Squeeze
)
```

