

- SwiftUI
- ModifiedContent
-  accessibility(identifier:) Deprecated

Instance Method

# accessibility(identifier:)

Uses the specified string to identify the view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func accessibility(identifier: String) -> ModifiedContent
```

Available when `Modifier` is `AccessibilityAttachmentModifier`.

Deprecated

Use accessibilityIdentifier(_:) instead.

## Discussion

Use this value for testing. It isn’t visible to the user.

