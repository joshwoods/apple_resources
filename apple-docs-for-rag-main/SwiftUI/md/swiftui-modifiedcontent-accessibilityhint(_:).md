

- SwiftUI
- ModifiedContent
-  accessibilityHint(\_:) 

Instance Method

# accessibilityHint(\_:)

Communicates to the user what happens after performing the view’s action.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func accessibilityHint(_ hint: Text) -> ModifiedContent
```

Available when `Modifier` is `AccessibilityAttachmentModifier`.

Show all declarations

## Discussion

Provide a hint in the form of a brief phrase, like “Purchases the item” or “Downloads the attachment”.

Note

On macOS, if the view does not have an action and it has been made into a container with `accessibilityElement(children: .contain)`, this will be used to describe the container. For example, if the container is for a graph, the hint could be “graph”.

