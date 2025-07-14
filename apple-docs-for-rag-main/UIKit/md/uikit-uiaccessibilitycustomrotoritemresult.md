

- UIKit
-  UIAccessibilityCustomRotorItemResult 

Class

# UIAccessibilityCustomRotorItemResult

A target element that a custom rotor references.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class UIAccessibilityCustomRotorItemResult
```

## Topics

### Creating a rotor item result

init(targetElement: any NSObjectProtocol, targetRange: UITextRange?)

Creates a rotor item result from the specified target element and text range.

### Getting information about the target element

var targetElement: (any NSObjectProtocol)?

The target element of the rotor.

var targetRange: UITextRange?

The text range (if any) of the target element.

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

class UIAccessibilityCustomRotorSearchPredicate

The search parameters that help determine the next matching custom rotor item result.

