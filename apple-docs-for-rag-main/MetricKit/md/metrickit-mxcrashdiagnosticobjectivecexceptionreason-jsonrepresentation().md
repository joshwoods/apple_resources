

- MetricKit
- MXCrashDiagnosticObjectiveCExceptionReason
-  jsonRepresentation() 

Instance Method

# jsonRepresentation()

Returns the contents of the exception reason in JSON format.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func jsonRepresentation() -> Data
```

## Return Value

An NSData object containing the JSON representation of the metrics in the payload.

## See Also

### Generating a report

func dictionaryRepresentation() -> [AnyHashable : Any]

