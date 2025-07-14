

- MetricKit
- MXMetaData
-  jsonRepresentation() 

Instance Method

# jsonRepresentation()

Returns the contents of the metadata in JSON format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
func jsonRepresentation() -> Data
```

## Return Value

A Data (Swift) or NSData (Objective-C) object containing the JSON representation of the contents of the metadata.

## See Also

### Generating a report

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the contents of the metadata as a dictionary.

Deprecated

