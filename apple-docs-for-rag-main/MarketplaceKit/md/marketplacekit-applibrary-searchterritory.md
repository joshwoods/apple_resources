

- MarketplaceKit
- AppLibrary
-  searchTerritory 

Instance Property

# searchTerritory

A country code that iOS uses to filter the search results of apps that aren’t available in that country.

iOS 17.4+iPadOS 17.4+

``` source
nonisolated
final var searchTerritory: String? { get async }
```

## Discussion

This property is an optional two-letter country code in the ISO 3166-1 alpha-2 standard that the alternative marketplace sets. For more information, see setSearchTerritory(_:).

## See Also

### Filtering app searches

func setSearchTerritory(String?) async

Defines a country code that iOS uses to filter the search results of apps that aren’t available in that country.

