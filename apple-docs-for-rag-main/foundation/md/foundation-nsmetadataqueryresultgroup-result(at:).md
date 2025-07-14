

- Foundation
- NSMetadataQueryResultGroup
-  result(at:) 

Instance Method

# result(at:)

Returns the query result at a specific index.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func result(at idx: Int) -> Any
```

## Parameters 

`idx`  

The index of the desired result.

## Return Value

The query result at a specific index.

## Discussion

For performance reasons, you should use this method when retrieving a specific result, rather than they array contained in results.

## See Also

### Getting Query Results

var attribute: String

The result group’s attribute name.

var value: Any

The result group’s value.

var results: [Any]

An array containing the result group’s result objects.

var resultCount: Int

The number of results returned by the result group.

var subgroups: [NSMetadataQueryResultGroup]?

An array containing the result group’s subgroups.

