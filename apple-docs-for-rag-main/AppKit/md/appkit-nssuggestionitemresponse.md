

- AppKit
-  NSSuggestionItemResponse 

Structure

# NSSuggestionItemResponse

Describes the result of a batch of suggestion items from a search

macOS 15.0+

``` source
struct NSSuggestionItemResponse
```

## Topics

### Initializers

init()

init(itemSections: [NSSuggestionItemResponse&lt;SuggestionItemType>.ItemSection])

init(items: [NSSuggestionItemResponse&lt;SuggestionItemType>.Item])

### Instance Properties

var itemSections: [NSSuggestionItemResponse&lt;SuggestionItemType>.ItemSection]

The items (organized in sections) representing the results of the search request

var phase: NSSuggestionItemResponse&lt;SuggestionItemType>.Phase

Describes the phase of results. In other words, whether this batch of items represents an intermediate set of results–and more are coming, or whether these results are complete/final. Defaults to `.final`.

var preferredHighlight: NSSuggestionItemResponse&lt;SuggestionItemType>.Highlight

The preferred response that the control should take when this batch of results comes in (like whether or not to highlight the first selectable item). Defaults to `.automatic`.

### Type Aliases

typealias Item

A suggestion item with the same suggestion item type as the response

typealias ItemSection

A suggestion item section with the same suggestion item type as the response

### Enumerations

enum Highlight

Describes the possible ways the highlighted item may be impacted by these results

enum Phase

Describes the different possible phases of results

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

