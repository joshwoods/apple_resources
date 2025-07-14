

- MetricKit
- MXDiagnostic
-  jsonRepresentation() 

Instance Method

# jsonRepresentation()

Returns the contents of the diagnostic in JSON format.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
func jsonRepresentation() -> Data
```

## Return Value

A Data (Swift) or NSData (Objective-C) object containing the JSON representation of the contents of the diagnostic.

## See Also

### Generating a report

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the contents of a diagnostic as a dictionary.

