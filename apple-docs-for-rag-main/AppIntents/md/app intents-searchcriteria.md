

- App Intents
-  SearchCriteria 

Protocol

# SearchCriteria

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
protocol SearchCriteria : _IntentValue, Hashable, Sendable
```

## Topics

### Associated Types

associatedtype SearchScopes = Void

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- StringSearchCriteria

## See Also

### Defining the search criteria

var criteria: Self.Criteria

**Required**

struct StringSearchCriteria

A structure that represents a string-based search request.

associatedtype Criteria : SearchCriteria

**Required**

