

- MetricKit
- MXDiagnostic
-  dictionaryRepresentation() 

Instance Method

# dictionaryRepresentation()

Returns the contents of a diagnostic as a dictionary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
func dictionaryRepresentation() -> [AnyHashable : Any]
```

## Return Value

A Dictionary (Swift) or NSDictionary (Objective-C) object containing the JSON representation of the contents of the diagnostic.

## See Also

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the diagnostic in JSON format.

