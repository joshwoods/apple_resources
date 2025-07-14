

- Core Services
- Search Kit
-  SKSearchOptions 

Type Alias

# SKSearchOptions

Specifies the search options available for the SKSearchCreate(_:_:_:) function.

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias SKSearchOptions = UInt32
```

## Topics

### Constants

var kSKSearchOptionDefault: Int

var kSKSearchOptionNoRelevanceScores: Int

This option saves time during a search by suppressing the computation of relevance scores.

var kSKSearchOptionSpaceMeansOR: Int

This option alters query behavior so that spaces are interpreted as Boolean `OR` operators.

var kSKSearchOptionFindSimilar: Int

This option alters query behavior so that Search Kit returns references to documents that are similar to an example text string. When this option is specified, Search Kit ignores all query operators.

