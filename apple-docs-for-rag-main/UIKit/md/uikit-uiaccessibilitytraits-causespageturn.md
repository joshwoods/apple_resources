

- UIKit
- UIAccessibilityTraits
-  causesPageTurn 

Type Property

# causesPageTurn

The accessibility element causes an automatic page turn when VoiceOver finishes reading the text within it.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let causesPageTurn: UIAccessibilityTraits
```

## Discussion

Use this trait to characterize an accessibility element that represents a page of content within a set of pages, such as a view that represents a page in a book. When VoiceOver finishes reading the content in the current page, it calls accessibilityScroll(_:) with UIAccessibilityScrollDirection.next to scroll to the next content page. If VoiceOver detects that the new content doesn’t differ from the previous content, it stops scrolling.

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

