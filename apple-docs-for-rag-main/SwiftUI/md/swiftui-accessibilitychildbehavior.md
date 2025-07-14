

- SwiftUI
-  AccessibilityChildBehavior 

Structure

# AccessibilityChildBehavior

Defines the behavior for the child elements of the new parent element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AccessibilityChildBehavior
```

## Topics

### Getting behaviors

static let combine: AccessibilityChildBehavior

Any child accessibility element’s properties are merged into the new accessibility element.

static let contain: AccessibilityChildBehavior

Any child accessibility elements become children of the new accessibility element.

static let ignore: AccessibilityChildBehavior

Any child accessibility elements become hidden.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Creating accessible elements

func accessibilityElement(children: AccessibilityChildBehavior) -> some View

Creates a new accessibility element, or modifies the AccessibilityChildBehavior of the existing accessibility element.

func accessibilityChildren&lt;V>(children: () -> V) -> some View

Replaces the existing accessibility element’s children with one or more new synthetic accessibility elements.

func accessibilityRepresentation&lt;V>(representation: () -> V) -> some View

Replaces one or more accessibility elements for this view with new accessibility elements.

