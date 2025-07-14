

- MetricKit
- MXDiagnosticPayload
-  dictionaryRepresentation() 

Instance Method

# dictionaryRepresentation()

Returns the results of the payload as a dictionary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
func dictionaryRepresentation() -> [AnyHashable : Any]
```

## Return Value

A Dictionary (Swift) or NSDictionary (Objective-C) object containing a key-value representation of the metrics in the payload.

## See Also

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the payload in JSON format.

