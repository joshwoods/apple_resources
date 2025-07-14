

- UIKit
- Accessibility for UIKit
-  UIAccessibility 

API Collection

# UIAccessibility

A set of methods that provides accessibility information about views and controls in an app’s user interface.

## Overview

The `UIAccessibility` informal protocol provides accessibility information about an app’s user interface elements. Assistive apps, such as VoiceOver, convey this information to users with disabilities to help them use the app.

Standard UIKit controls and views implement the `UIAccessibility` methods and are accessible to assistive apps by default. This means that if your app uses only standard controls and views, such as UIButton, UISegmentedControl, and UITableView, you need only supply app-specific details when the default values are incomplete. You can do this by setting these values in Interface Builder or by setting the properties in this informal protocol.

The UIAccessibilityElement class, which represents custom user interface objects, also implements the `UIAccessibility` informal protocol. If you create a completely custom UIView subclass, you might need to create an instance of UIAccessibilityElement to represent it. In this case, you’d support all the `UIAccessibility` properties to correctly set and return the accessibility element’s properties.

## Topics

### Supporting basic accessibility

@MainActor var isAccessibilityElement: Bool { get set }

@MainActor var accessibilityLabel: String? { get set }

@MainActor var accessibilityValue: String? { get set }

@MainActor var accessibilityHint: String? { get set }

@MainActor var accessibilityTraits: UIAccessibilityTraits { get set }

struct UIAccessibilityTraits

Constants that describe how an accessibility element behaves.

### Defining accessibility text and language

Speech attributes for attributed strings

Apply attributes to text in an attributed string to modify the pronunciation of that text.

Text attributes for attributed strings

Apply attributes to text in an attributed string to convey extra information about the text.

@MainActor var accessibilityHeaderElements: [Any]? { get set }

@MainActor @NSCopying var accessibilityAttributedHint: NSAttributedString? { get set }

@MainActor @NSCopying var accessibilityAttributedLabel: NSAttributedString? { get set }

@MainActor var accessibilityLanguage: String? { get set }

@MainActor var accessibilityTextualContext: UIAccessibilityTextualContext? { get set }

@MainActor var accessibilityUserInputLabels: [String]! { get set }

@MainActor var accessibilityAttributedUserInputLabels: [NSAttributedString]! { get set }

@MainActor @NSCopying var accessibilityAttributedValue: NSAttributedString? { get set }

### Configuring behavior

@MainActor var accessibilityCustomRotors: [UIAccessibilityCustomRotor]? { get set }

@MainActor var accessibilityElementsHidden: Bool { get set }

@MainActor var accessibilityRespondsToUserInteraction: Bool { get set }

@MainActor var accessibilityViewIsModal: Bool { get set }

@MainActor var shouldGroupAccessibilityChildren: Bool { get set }

@MainActor var accessibilityDirectTouchOptions: UIAccessibility.DirectTouchOptions { get set }

struct DirectTouchOptions

Constants that configure how VoiceOver produces audio for direct touch areas.

### Handling notifications

Notification names

The names of notifications that the accessibility system generates.

Notification dictionary keys

Handle notifications with keys in the user info dictionary.

struct Notification

An accessibility notification that an app can send.

static func post(notification: UIAccessibility.Notification, argument: Any?)

Posts a notification to assistive apps.

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

enum ZoomType

The types of system Zoom that can be in effect.

static var assistiveTouch: UIGuidedAccessAccessibilityFeature

The AssistiveTouch accessibility feature.

### Supporting types

typealias AXArrayReturnBlock

typealias AXAttributedStringArrayReturnBlock

typealias AXAttributedStringReturnBlock

typealias AXBoolReturnBlock

typealias AXContainerTypeReturnBlock

typealias AXCustomActionsReturnBlock

typealias AXCustomRotorsReturnBlock

typealias AXNavigationStyleReturnBlock

typealias AXObjectReturnBlock

typealias AXPathReturnBlock

typealias AXPointReturnBlock

typealias AXRectReturnBlock

typealias AXStringArrayReturnBlock

typealias AXStringReturnBlock

typealias AXTextualContextReturnBlock

typealias AXTraitsReturnBlock

typealias AXUITextInputReturnBlock

typealias AXVoidReturnBlock

struct UIAccessibility

A namespace for accessibility symbols for UIKit apps.

## See Also

### Related Documentation

Accessibility

Make your apps accessible to everyone who uses Apple devices.

Accessibility for UIKit

Make your UIKit apps accessible to everyone who uses iOS and tvOS.

### Essentials

UIAccessibilityContainer

Provide a set of methods that view subclasses use to make subcomponents accessible as separate elements.

Supporting VoiceOver in your app

Add VoiceOver support to make your iOS app more accessible to users who are blind or have low vision.

