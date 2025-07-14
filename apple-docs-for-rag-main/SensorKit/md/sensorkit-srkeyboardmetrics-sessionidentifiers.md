

- SensorKit
- SRKeyboardMetrics
-  sessionIdentifiers 

Instance Property

# sessionIdentifiers

The identifiers for the keyboard sessions that report metrics to the sample.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var sessionIdentifiers: [String] { get }
```

## Discussion

A keyboard session begins when the system presents the keyboard and ends when the system dismisses it.

## See Also

### Inspecting Keyboard Configuration and Sessions

var duration: TimeInterval

The duration that the report spans.

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

