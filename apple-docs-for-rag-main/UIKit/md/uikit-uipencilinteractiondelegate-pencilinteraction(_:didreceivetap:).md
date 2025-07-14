

- UIKit
- UIPencilInteractionDelegate
-  pencilInteraction(\_:didReceiveTap:) 

Instance Method

# pencilInteraction(\_:didReceiveTap:)

Tells the delegate when a person double-taps Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
optional func pencilInteraction(
    _ interaction: UIPencilInteraction,
    didReceiveTap tap: UIPencilInteraction.Tap
)
```

