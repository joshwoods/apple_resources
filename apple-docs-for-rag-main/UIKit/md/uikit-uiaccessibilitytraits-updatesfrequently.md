

- UIKit
- UIAccessibilityTraits
-  updatesFrequently 

Type Property

# updatesFrequently

The accessibility element frequently updates its label or value.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
nonisolated
static let updatesFrequently: UIAccessibilityTraits
```

## Discussion

Use this trait to characterize an accessibility element that updates its label or value too frequently to send update notifications. Include this trait when you want an assistive app to avoid handling continual notifications and, instead, poll for changes when it needs updated information. For example, you might use this trait to characterize the readout of a stopwatch.

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

