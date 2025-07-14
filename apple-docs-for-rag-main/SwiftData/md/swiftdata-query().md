

- SwiftData
-  Query() 

Macro

# Query()

Fetches all instances of the attached model type.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(accessor) @attached(peer, names: prefixed(`_`))
macro Query()
```

## See Also

### Model fetch

Filtering and sorting persistent data

Manage data store presentation using predicates and dynamic queries.

Additional query macros

Supplementary macros that enable you to narrow query results and tell SwiftData how to sort and order those results.

struct Query

A type that fetches models using the specified criteria, and manages those models so they remain in sync with the underlying data.

struct FetchDescriptor

A type that describes the criteria, sort order, and any additional configuration to use when performing a fetch.

