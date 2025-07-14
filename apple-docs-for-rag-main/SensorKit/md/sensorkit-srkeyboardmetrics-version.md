

- SensorKit
- SRKeyboardMetrics
-  version 

Instance Property

# version

The version of keyboard metrics.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var version: String { get }
```

## See Also

### Inspecting Keyboard Configuration and Sessions

var duration: TimeInterval

The duration that the report spans.

var keyboardIdentifier: String

The identifier of the keyboard in the keyboard list.

var width: Measurement&lt;UnitLength>

The width, in millimeters, of the keyboard in the report.

var height: Measurement&lt;UnitLength>

The height, in millimeters, of the keyboard in the report.

var inputModes: [String]

The active keyboard languages in the session.

var sessionIdentifiers: [String]

The identifiers for the keyboard sessions that report metrics to the sample.

