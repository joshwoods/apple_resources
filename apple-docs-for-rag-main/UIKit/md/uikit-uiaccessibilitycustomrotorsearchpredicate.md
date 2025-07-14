

- UIKit
-  UIAccessibilityCustomRotorSearchPredicate 

Class

# UIAccessibilityCustomRotorSearchPredicate

The search parameters that help determine the next matching custom rotor item result.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class UIAccessibilityCustomRotorSearchPredicate
```

## Topics

### Configuring search parameters

var currentItem: UIAccessibilityCustomRotorItemResult

The current element of the search.

var searchDirection: UIAccessibilityCustomRotor.Direction

The direction in which to search.

enum Direction

Constants that indicate the search direction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Navigation

class UIAccessibilityCustomRotor

A context-sensitive function that helps VoiceOver users find the next instance of a related element.

class UIAccessibilityCustomRotorItemResult

A target element that a custom rotor references.

