

- AppKit
-  NSSuggestionItemSection 

Structure

# NSSuggestionItemSection

Describes a section of suggestions items in a suggestions menu

macOS 15.0+

``` source
struct NSSuggestionItemSection
```

## Topics

### Initializers

init(items: [NSSuggestionItemSection&lt;SuggestionItemType>.Item])

init(title: String?, items: [NSSuggestionItemSection&lt;SuggestionItemType>.Item])

### Instance Properties

var items: [NSSuggestionItemSection&lt;SuggestionItemType>.Item]

The items that appear in this section

var title: String?

The title of this section of items, or `nil` to have a untitled section of items

### Type Aliases

typealias Item

A suggestion item with the same suggestion item type as the section

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

