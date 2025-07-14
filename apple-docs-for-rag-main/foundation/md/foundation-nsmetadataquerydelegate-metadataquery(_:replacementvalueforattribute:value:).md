

- Foundation
- NSMetadataQueryDelegate
-  metadataQuery(\_:replacementValueForAttribute:value:) 

Instance Method

# metadataQuery(\_:replacementValueForAttribute:value:)

Returns a different value for a given attribute and value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func metadataQuery(
    _ query: NSMetadataQuery,
    replacementValueForAttribute attrName: String,
    value attrValue: Any
) -> Any
```

## Parameters 

`query`  

The query that produced the result object with `attrName`.

`attrName`  

The attribute in question.

`attrValue`  

The attribute value to replace.

## Return Value

Object that replaces the value of `attrName` in the result object

## Discussion

The delegate implementation of this method could convert specific query attribute values to other attribute values, for example, converting date object values to formatted strings for display.

## See Also

### Getting Query Results

func metadataQuery(NSMetadataQuery, replacementObjectForResultObject: NSMetadataItem) -> Any

Returns a different object for a given query result object.

