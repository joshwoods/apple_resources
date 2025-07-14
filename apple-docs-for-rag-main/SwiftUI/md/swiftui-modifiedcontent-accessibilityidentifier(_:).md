

- SwiftUI
- ModifiedContent
-  accessibilityIdentifier(\_:) 

Instance Method

# accessibilityIdentifier(\_:)

Uses the string you specify to identify the view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func accessibilityIdentifier(_ identifier: String) -> ModifiedContent
```

Available when `Modifier` is `AccessibilityAttachmentModifier`.

## Discussion

Use this value for testing. It isn’t visible to the user.

