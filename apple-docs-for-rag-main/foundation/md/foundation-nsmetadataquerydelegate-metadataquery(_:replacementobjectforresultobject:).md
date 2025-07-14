

- Foundation
- NSMetadataQueryDelegate
-  metadataQuery(\_:replacementObjectForResultObject:) 

Instance Method

# metadataQuery(\_:replacementObjectForResultObject:)

Returns a different object for a given query result object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func metadataQuery(
    _ query: NSMetadataQuery,
    replacementObjectForResultObject result: NSMetadataItem
) -> Any
```

## Parameters 

`query`  

The query that produced the result object to replace.

`result`  

The query result object to replace.

## Return Value

Object that replaces the query result object.

## Discussion

By default query result objects are instances of the NSMetadataItem class. By implementing this method, you can return an object of a different class type for the specified result object.

## See Also

### Related Documentation

File Metadata Search Programming Guide

### Getting Query Results

func metadataQuery(NSMetadataQuery, replacementValueForAttribute: String, value: Any) -> Any

Returns a different value for a given attribute and value.

