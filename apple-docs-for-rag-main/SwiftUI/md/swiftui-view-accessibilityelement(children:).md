

- SwiftUI
- View
-  accessibilityElement(children:) 

Instance Method

# accessibilityElement(children:)

Creates a new accessibility element, or modifies the AccessibilityChildBehavior of the existing accessibility element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func accessibilityElement(children: AccessibilityChildBehavior = .ignore) -> some View
```

## Parameters 

`children`  

The behavior to use when creating or transforming an accessibility element. The default is ignore

## Discussion

See also:

- ignore

- combine

- contain

## See Also

### Creating accessible elements

func accessibilityChildren&lt;V>(children: () -> V) -> some View

Replaces the existing accessibility element’s children with one or more new synthetic accessibility elements.

func accessibilityRepresentation&lt;V>(representation: () -> V) -> some View

Replaces one or more accessibility elements for this view with new accessibility elements.

struct AccessibilityChildBehavior

Defines the behavior for the child elements of the new parent element.

