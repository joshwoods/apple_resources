

- Foundation
- NSMetadataQueryResultGroup
-  subgroups 

Instance Property

# subgroups

An array containing the result group’s subgroups.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var subgroups: [NSMetadataQueryResultGroup]? { get }
```

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

func result(at: Int) -> Any

Returns the query result at a specific index.

