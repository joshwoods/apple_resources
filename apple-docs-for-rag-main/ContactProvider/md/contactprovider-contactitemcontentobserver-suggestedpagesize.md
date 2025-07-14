

- ContactProvider
- ContactItemContentObserver
-  suggestedPageSize 

Instance Property

# suggestedPageSize

Retrieves the suggested number of items to include in a page.

iOS 18.0+iPadOS 18.0+

``` source
var suggestedPageSize: Int { get }
```

**Required**

## Discussion

This value is a suggested upper limit for the number of contact items you can pass in the aggregate calls to didEnumerate(_:). Exceeding this limit may result in memory issues.

