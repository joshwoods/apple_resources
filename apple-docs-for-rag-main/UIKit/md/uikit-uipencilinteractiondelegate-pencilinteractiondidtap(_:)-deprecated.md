

- UIKit
- UIPencilInteractionDelegate
-  pencilInteractionDidTap(\_:) Deprecated

Instance Method

# pencilInteractionDidTap(\_:)

Tells the delegate that the user double-tapped Apple Pencil.

iOS 12.1–17.5DeprecatediPadOS 12.1–17.5DeprecatedMac Catalyst 13.1–17.5Deprecated

``` source
@MainActor
optional func pencilInteractionDidTap(_ interaction: UIPencilInteraction)
```

Deprecated

Use pencilInteraction(_:didReceiveTap:) instead.

## Discussion

When handling the double tap, perform either:

- The action selected by the user in the Settings app, as specified by the preferredTapAction class property.

- An alternative behavior that gives the user the best experience for your app. Should you decide to support an alternative, provide an intuitive way for the user to learn about and enable that behavior.

