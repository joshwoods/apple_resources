

- AppKit
- NSSuggestionItemResponse
-  NSSuggestionItemResponse.Phase 

Enumeration

# NSSuggestionItemResponse.Phase

Describes the different possible phases of results

macOS 15.0+

``` source
enum Phase
```

## Topics

### Enumeration Cases

case final

The collection of items represents a final set of results for the request. The user can expect these results to be stable until their search request changes.

case intermediate

The collection of items represent an intermediate (non-final) set of results. The user can expect to potentially see more results in a short period of time.

## Relationships

### Conforms To

- Equatable
- Hashable

