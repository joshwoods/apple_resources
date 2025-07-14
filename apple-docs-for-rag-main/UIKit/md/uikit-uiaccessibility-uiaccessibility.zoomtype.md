

- UIKit
- UIAccessibility
-  UIAccessibility.ZoomType 

Enumeration

# UIAccessibility.ZoomType

The types of system Zoom that can be in effect.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum ZoomType
```

## Topics

### Constants

case insertionPoint

The system zoom type is the text insertion point.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Navigating elements

UIAccessibilityContainer

Provide a set of methods that view subclasses use to make subcomponents accessible as separate elements.

@MainActor var accessibilityActivationPoint: CGPoint { get set }

var accessibilityFocusedUIElement: Any? { get }

@MainActor var accessibilityFrame: CGRect { get set }

func accessibilityHitTest(_ point: NSPoint) -> Any?

@MainActor var accessibilityNavigationStyle: UIAccessibilityNavigationStyle { get set }

enum UIAccessibilityNavigationStyle

Constants that describe how to navigate an object’s elements with an assistive app.

@MainActor @NSCopying var accessibilityPath: UIBezierPath? { get set }

static func zoomFocusChanged(zoomType: UIAccessibility.ZoomType, toFrame: CGRect, in: UIView)

Notifies the system when the app’s focus changes to a new location.

static var assistiveTouch: UIGuidedAccessAccessibilityFeature

The AssistiveTouch accessibility feature.

