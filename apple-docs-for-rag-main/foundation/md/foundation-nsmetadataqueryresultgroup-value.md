

- Foundation
- NSMetadataQueryResultGroup
-  value 

Instance Property

# value

The result group’s value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var value: Any { get }
```

## See Also

### Getting Query Results

var attribute: String

The result group’s attribute name.

var results: [Any]

An array containing the result group’s result objects.

var resultCount: Int

The number of results returned by the result group.

func result(at: Int) -> Any

Returns the query result at a specific index.

var subgroups: [NSMetadataQueryResultGroup]?

An array containing the result group’s subgroups.

