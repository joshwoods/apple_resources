

- MetricKit
- MXMetricPayload
-  dictionaryRepresentation() Deprecated

Instance Method

# dictionaryRepresentation()

Returns the results of the payload as a dictionary.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1+visionOS 1.0–2.4Deprecated

``` source
func dictionaryRepresentation() -> [AnyHashable : Any]
```

Deprecated

Use dictionaryRepresentation() instead.

## Return Value

A Dictionary (Swift) or NSDictionary (Objective-C) object containing a key-value representation of the metrics in the payload.

## See Also

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the payload in JSON format.

