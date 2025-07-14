

- UIKit
-  UIAccessibilityNavigationStyle 

Enumeration

# UIAccessibilityNavigationStyle

Constants that describe how to navigate an object’s elements with an assistive app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum UIAccessibilityNavigationStyle
```

## Topics

### Constants

case automatic

The assistive technology automatically determines how the receiver’s elements should be navigated.

case separate

The receiver’s elements should be navigated as separate elements.

case combined

The receiver’s elements should be combined and navigated as a single item.

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

@MainActor @NSCopying var accessibilityPath: UIBezierPath? { get set }

static func zoomFocusChanged(zoomType: UIAccessibility.ZoomType, toFrame: CGRect, in: UIView)

Notifies the system when the app’s focus changes to a new location.

enum ZoomType

The types of system Zoom that can be in effect.

static var assistiveTouch: UIGuidedAccessAccessibilityFeature

The AssistiveTouch accessibility feature.

