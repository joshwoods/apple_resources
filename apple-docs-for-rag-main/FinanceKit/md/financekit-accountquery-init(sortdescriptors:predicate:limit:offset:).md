

- FinanceKit
- AccountQuery
-  init(sortDescriptors:predicate:limit:offset:) 

Initializer

# init(sortDescriptors:predicate:limit:offset:)

Creates a new account query structure with the provided sort descriptors and, optionally, a predicate and limit on the number of records the query should return.

iOS 17.4+iPadOS 17.4+

``` source
init(
    sortDescriptors: [SortDescriptor] = [],
    predicate: Predicate? = nil,
    limit: Int? = nil,
    offset: Int? = nil
)
```

## Parameters 

`sortDescriptors`  

An array of Account sort descriptors.

`predicate`  

A Predicate to filter the `Account` records with.

`limit`  

An integer that indicates the maximum number of `Account` records to return.

`offset`  

An integer that indicates the number of records to offset the result by.

