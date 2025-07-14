

- SwiftUI
- View
-  accessibilityLabel(content:) 

Instance Method

# accessibilityLabel(content:)

Adds a label to the view that describes its contents.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityLabel(@ViewBuilder content: (PlaceholderContentView) -> V) -> some View where V : View
```

## Parameters 

`content`  

A view builder closure that takes a proxy value representing the modified view. You can combine the modified view with other content to create a new accessibility label for the original view.

## Discussion

Use this method to append content to the accessibility label for a view. For example, you could use this method to label a badge or alert that is custom drawn without removing the existing accessibility label.

## See Also

### Applying labels

func accessibilityLabel(_:)

Adds a label to the view that describes its contents.

func accessibilityLabel(_:isEnabled:)

Adds a label to the view that describes its contents.

func accessibilityInputLabels(_:)

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels(_:isEnabled:)

Sets alternate input labels with which users identify a view.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

enum AccessibilityLabeledPairRole

The role of an accessibility element in a label / content pair.

