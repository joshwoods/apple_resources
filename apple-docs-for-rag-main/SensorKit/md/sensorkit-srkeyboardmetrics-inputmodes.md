

- SensorKit
- SRKeyboardMetrics
-  inputModes 

Instance Property

# inputModes

The active keyboard languages in the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var inputModes: [String] { get }
```

## Discussion

An example array entry is `en_US`. A user may switch between multiple languages in the same session.

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

var sessionIdentifiers: [String]

The identifiers for the keyboard sessions that report metrics to the sample.

