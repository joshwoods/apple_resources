

- Foundation
- NSMetadataQueryResultGroup
-  results 

Instance Property

# results

An array containing the result group’s result objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var results: [Any] { get }
```

## Discussion

The results array is a proxy object that is primarily intended for use with Cocoa bindings. While it is possible to copy the proxy array to get a “snapshot” of the complete current query results, it is generally not recommended due to performance and memory issues. To access individual result array elements you should instead use the resultCount property and the result(at:) method.

## See Also

### Getting Query Results

var attribute: String

The result group’s attribute name.

var value: Any

The result group’s value.

var resultCount: Int

The number of results returned by the result group.

func result(at: Int) -> Any

Returns the query result at a specific index.

var subgroups: [NSMetadataQueryResultGroup]?

An array containing the result group’s subgroups.

