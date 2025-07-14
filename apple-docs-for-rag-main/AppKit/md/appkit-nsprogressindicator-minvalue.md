

- AppKit
- NSProgressIndicator
-  minValue 

Instance Property

# minValue

The minimum value for the progress indicator.

macOS

``` source
@MainActor
var minValue: Double { get set }
```

## Discussion

By default, a determinate progress indicator goes from `0.0` to `100.0`, so the default value of this property is `0.0`.

An indeterminate progress indicator does not use this value.

## See Also

### Advancing the progress bar

func increment(by: Double)

Advances the progress bar of a determinate progress indicator by the specified amount.

var doubleValue: Double

The value that indicates the current extent of the progress indicator.

var maxValue: Double

The maximum value for the progress indicator.

