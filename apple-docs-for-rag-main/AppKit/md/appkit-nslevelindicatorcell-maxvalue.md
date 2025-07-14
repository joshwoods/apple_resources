

- AppKit
- NSLevelIndicatorCell
-  maxValue 

Instance Property

# maxValue

The maximum value of the control.

macOS

``` source
@MainActor
var maxValue: Double { get set }
```

## Discussion

The maximum value is dependent on the style of the control. For continuous styles, the default value of this property is `100.0`. For discrete styles, the default maximum value is `5.0`.

## See Also

### Configuring the Range of Values

var minValue: Double

The minimum value of the control.

var levelIndicatorStyle: NSLevelIndicator.Style

The style of the level indicator control.

var warningValue: Double

The warning value of the level indicator control.

var criticalValue: Double

The critical value of the level indicator control.

