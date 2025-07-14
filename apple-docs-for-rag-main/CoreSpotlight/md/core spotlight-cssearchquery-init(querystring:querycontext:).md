

- Core Spotlight
- CSSearchQuery
-  init(queryString:queryContext:) 

Initializer

# init(queryString:queryContext:)

Initializes and returns a query object with the specified query string and query context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    queryString: String,
    queryContext: CSSearchQueryContext?
)
```

## Return Value

An initialized query object.

## Discussion

- queryString: A formatted string that defines the matching criteria to apply to indexed items. To learn how to construct a query string, see Create a query string for your search.

  This parameter must not be `nil`.

  - queryContext: A CSSearchQueryContext object that focuses the query results.

## Discussion

After you create and initialize a query object, and call start() to begin the query, you can’t update or reuse the query object for a new query.

## See Also

### Creating a query object

convenience init(queryString: String, attributes: [String]?)

Initializes and returns a query object with the specified query string and item attributes.

Deprecated

