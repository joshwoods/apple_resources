

- AppKit
-  NSSuggestionItem 

Structure

# NSSuggestionItem

The items that appear in suggestion menus.

macOS 15.0+

``` source
struct NSSuggestionItem
```

## Topics

### Initializers

init(representedValue: SuggestionItemType, attributedTitle: AttributedString)

init(representedValue: SuggestionItemType, title: String)

### Instance Properties

var attributedSecondaryTitle: AttributedString?

An optional second attributed string to display for a suggestion menu item. This value should be localized. This value is an attributed string representation of `secondaryTitle`.

var attributedTitle: AttributedString

An attributed string to display for a suggestion menu item. This value should be localized. This value is an attributed string representation of `title`.

var image: NSImage?

An optional image to display before the title. This value should be localized.

var representedValue: SuggestionItemType

The value represented by the receiver.

var secondaryTitle: String?

An optional second string to display for a suggestion menu item. This value should be localized. This value is a non-attributed string representation of `attributedSecondaryTitle`.

var title: String

A string to display for a suggestion menu item. This value should be localized. This value is a non-attributed string representation of `attributedTitle`.

var toolTip: String?

An optional tool tip to display on hover for a suggestion menu item. This value should be localized.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

