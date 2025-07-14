

- Foundation
-  NSMetadataQueryDelegate 

Protocol

# NSMetadataQueryDelegate

An interface that enables the delegate of a metadata query to provide substitute results or attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSMetadataQueryDelegate : NSObjectProtocol
```

## Topics

### Getting Query Results

func metadataQuery(NSMetadataQuery, replacementObjectForResultObject: NSMetadataItem) -> Any

Returns a different object for a given query result object.

func metadataQuery(NSMetadataQuery, replacementValueForAttribute: String, value: Any) -> Any

Returns a different value for a given attribute and value.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### File Search

class NSMetadataQuery

A query that you perform against Spotlight metadata.

class NSMetadataItem

The metadata associated with a file.

