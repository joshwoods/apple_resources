

- UIKit
- UIAccessibilityTraits
-  toggleButton 

Type Property

# toggleButton

The accessibility element behaves like a toggle button.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
static let toggleButton: UIAccessibilityTraits
```

## Discussion

Use this trait to characterize an accessibility element that represents a button that toggles a value on, off, or mixed status. VoiceOver will describe the options offered by the toggle button.

Note

If you want VoiceOver to describe the toggle as a switch button, combine the toggle trait with a button trait.

## See Also

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

