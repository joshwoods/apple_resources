

- Core Spotlight
- CSSearchQuery
-  init(queryString:attributes:) Deprecated

Initializer

# init(queryString:attributes:)

Initializes and returns a query object with the specified query string and item attributes.

iOS 10.0–16.0DeprecatediPadOS 10.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.13–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init(
    queryString: String,
    attributes: [String]?
)
```

Deprecated

Use initWithQueryString:queryContext instead

## Return Value

An initialized query object.

## Discussion

- queryString: A formatted string that defines the matching criteria to apply to indexed items. To learn how to construct a query string, see Create a query string for your search.

  This parameter must not be `nil`.

  - attributes: An array of strings that represent the attributes of indexed items. Each string corresponds to a property name that your app can set for an item; for a list of possible properties, see CSSearchableItemAttributeSet. Passing `nil` for this parameter means that the query doesn’t use attributes to find matching items.

## Discussion

After you create and initialize a query object, and call start() to begin the query, you can’t update or reuse the query object for a new query.

## See Also

### Creating a query object

init(queryString: String, queryContext: CSSearchQueryContext?)

Initializes and returns a query object with the specified query string and query context.

