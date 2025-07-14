

- TabularData
- RowGroupingProtocol
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns a row grouping containing only the groups that satisfy a predicate.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
func filter(_ isIncluded: (DataFrame.Slice) throws -> Bool) rethrows -> Self
```

**Required**

## Parameters 

`isIncluded`  

A predicate closure that takes a group and returns a Boolean that indicates whether the group is included.

## Return Value

A data frame slice that contains the rows that satisfy the predicate.

