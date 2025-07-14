

- Core Services
- Search Kit
-  SKSearchType 

Structure

# SKSearchType

Search Kit ignores the constants in this group. Use asynchronous searching with `SKSearchCreate` instead, which uses query syntax to determine search type.

Mac Catalyst 13.0+macOS 10.3+

``` source
struct SKSearchType
```

## Overview

In releases of macOS prior to version 10.4, these constants specify the category of search to perform. Starting with OS X v10.4, use asynchronous searching with `SKSearchCreate` instead, which uses query syntax to determine search type.

In older versions of macOS, these constants specify the various search types you can use with `SKSearchResultsCreateWithQuery`. Each of these specifies a set of ranked search hits. The `kSKSearchRanked` and `kSKSearchPrefixRanked` constants can be used for all index types. The `kSKSearchBooleanRanked` and `kSKSearchRequiredRanked` constants cannot be used for vector indexes.

## Topics

### Constants

var kSKSearchRanked: SKSearchType

Deprecated. Specifies a basic ranked search.

var kSKSearchBooleanRanked: SKSearchType

Deprecated. Specifies a query that can include Boolean operators including `'|'`, `'&'`, `'!'`, `'('`, and `')'`.

var kSKSearchRequiredRanked: SKSearchType

Deprecated. Specifies a query that can include required (`'+'`) or excluded (`'-'`) terms.

var kSKSearchPrefixRanked: SKSearchType

Deprecated. Specifies a prefix-based search, which matches terms that begin with the query string.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- Hashable
- RawRepresentable

