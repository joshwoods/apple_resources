

- App Intents
- ShowInAppSearchResultsIntent
-  searchScopes 

Type Property

# searchScopes

Values that help the system understand the scope of an app intent that shows the results of a string-based search.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
static var searchScopes: Self.Criteria.SearchScopes { get }
```

**Required** Default implementations provided.

## Default Implementations

### ShowInAppSearchResultsIntent Implementations

static var searchScopes: Void

static var searchScopes: [StringSearchScope]

A default value that helps the system understand the scope of an app intent that shows the results of a string-based search.

## See Also

### Scoping the search

enum StringSearchScope

Constants that help the system understand the in-app search functionality and its searchable content.

