

- SwiftUI
- View
-  accessibilityRemoveTraits(\_:) 

Instance Method

# accessibilityRemoveTraits(\_:)

Removes the given traits from this view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func accessibilityRemoveTraits(_ traits: AccessibilityTraits) -> ModifiedContent
```

## See Also

### Assigning traits to content

func accessibilityAddTraits(AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds the given traits to the view.

struct AccessibilityTraits

A set of accessibility traits that describe how an element behaves.

