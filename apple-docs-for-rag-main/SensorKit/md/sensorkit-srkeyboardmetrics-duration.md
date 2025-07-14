

- SensorKit
- SRKeyboardMetrics
-  duration 

Instance Property

# duration

The duration that the report spans.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var duration: TimeInterval { get }
```

## See Also

### Inspecting Keyboard Configuration and Sessions

var keyboardIdentifier: String

The identifier of the keyboard in the keyboard list.

var version: String

The version of keyboard metrics.

var width: Measurement&lt;UnitLength>

The width, in millimeters, of the keyboard in the report.

var height: Measurement&lt;UnitLength>

The height, in millimeters, of the keyboard in the report.

var inputModes: [String]

The active keyboard languages in the session.

var sessionIdentifiers: [String]

The identifiers for the keyboard sessions that report metrics to the sample.

