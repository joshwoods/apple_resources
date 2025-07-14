

- AppKit
- NSLevelIndicatorCell
-  levelIndicatorStyle 

Instance Property

# levelIndicatorStyle

The style of the level indicator control.

macOS

``` source
@MainActor
var levelIndicatorStyle: NSLevelIndicator.Style { get set }
```

## Discussion

The style determines the default minimum and maximum values of the control. For a list of possible styles, see NSLevelIndicator.Style.

## See Also

### Configuring the Range of Values

var minValue: Double

The minimum value of the control.

var maxValue: Double

The maximum value of the control.

var warningValue: Double

The warning value of the level indicator control.

var criticalValue: Double

The critical value of the level indicator control.

