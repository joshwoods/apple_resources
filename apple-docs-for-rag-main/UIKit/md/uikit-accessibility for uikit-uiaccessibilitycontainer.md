

- UIKit
- Accessibility for UIKit
-  UIAccessibilityContainer 

API Collection

# UIAccessibilityContainer

Provide a set of methods that view subclasses use to make subcomponents accessible as separate elements.

## Topics

### Providing information about accessibility elements

@MainActor func accessibilityElementCount() -> Int

@MainActor func accessibilityElement(at index: Int) -> Any?

@MainActor func index(ofAccessibilityElement element: Any) -> Int

@MainActor var accessibilityElements: [Any]? { get set }

@MainActor var automationElements: [Any]? { get set }

@MainActor var accessibilityContainerType: UIAccessibilityContainerType { get set }

enum UIAccessibilityContainerType

Constants that indicate the type of content in a data-based container.

### Useful links

Accessibility design for Mac Catalyst

Improve navigation in your app by using keyboard shortcuts and accessibility containers.

## See Also

### Essentials

UIAccessibility

A set of methods that provides accessibility information about views and controls in an app’s user interface.

Supporting VoiceOver in your app

Add VoiceOver support to make your iOS app more accessible to users who are blind or have low vision.

