

- UIKit
-  UIAccessibilityTraits 

Structure

# UIAccessibilityTraits

Constants that describe how an accessibility element behaves.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
struct UIAccessibilityTraits
```

## Overview

Set these traits to tell an assistive app how an accessibility element behaves or how to treat it.

## Topics

### Constants

static let none: UIAccessibilityTraits

The accessibility element has no traits.

static let button: UIAccessibilityTraits

The accessibility element behaves like a button.

static let link: UIAccessibilityTraits

The accessibility element behaves like a link.

static let image: UIAccessibilityTraits

The accessibility element behaves like an image.

static let searchField: UIAccessibilityTraits

The accessibility element behaves like a search field.

static let toggleButton: UIAccessibilityTraits

The accessibility element behaves like a toggle button.

static let keyboardKey: UIAccessibilityTraits

The accessibility element behaves like a keyboard key.

static let staticText: UIAccessibilityTraits

The accessibility element behaves like static text that can’t change.

static let header: UIAccessibilityTraits

The accessibility element is a header that divides content into sections, such as the title of a navigation bar.

static let tabBar: UIAccessibilityTraits

The accessibility element behaves like a tab bar.

static let summaryElement: UIAccessibilityTraits

The accessibility element provides summary information when the app starts.

static let selected: UIAccessibilityTraits

The accessibility element is currently in a selected state.

static let notEnabled: UIAccessibilityTraits

The accessibility element isn’t in an enabled state and doesn’t respond to user interaction.

static let adjustable: UIAccessibilityTraits

The accessibility element allows continuous adjustment through a range of values.

static let allowsDirectInteraction: UIAccessibilityTraits

The accessibility element allows direct touch interaction for VoiceOver users.

static let updatesFrequently: UIAccessibilityTraits

The accessibility element frequently updates its label or value.

static let causesPageTurn: UIAccessibilityTraits

The accessibility element causes an automatic page turn when VoiceOver finishes reading the text within it.

static let playsSound: UIAccessibilityTraits

The accessibility element plays its own sound when the user activates it.

static let startsMediaSession: UIAccessibilityTraits

The accessibility element starts a media session when the user activates it.

static let supportsZoom: UIAccessibilityTraits

The accessibility element supports zooming in and out on its content.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Supporting basic accessibility

@MainActor var isAccessibilityElement: Bool { get set }

@MainActor var accessibilityLabel: String? { get set }

@MainActor var accessibilityValue: String? { get set }

@MainActor var accessibilityHint: String? { get set }

@MainActor var accessibilityTraits: UIAccessibilityTraits { get set }

