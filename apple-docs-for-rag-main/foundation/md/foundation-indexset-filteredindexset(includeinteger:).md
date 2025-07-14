

- Foundation
- IndexSet
-  filteredIndexSet(includeInteger:) 

Instance Method

# filteredIndexSet(includeInteger:)

Returns an IndexSet filtered according to the result of `includeInteger`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func filteredIndexSet(includeInteger: (IndexSet.Element) throws -> Bool) rethrows -> IndexSet
```

## Parameters 

`includeInteger`  

The predicate which decides if an integer will be included in the result or not.

## See Also

### Selecting Elements

func filteredIndexSet(in: Range&lt;IndexSet.Element>, includeInteger: (IndexSet.Element) throws -> Bool) rethrows -> IndexSet

Returns an IndexSet filtered according to the result of `includeInteger`.

func filteredIndexSet(in: ClosedRange&lt;IndexSet.Element>, includeInteger: (IndexSet.Element) throws -> Bool) rethrows -> IndexSet

Returns an IndexSet filtered according to the result of `includeInteger`.

