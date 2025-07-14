

- AppKit
- NSProgressIndicator
-  doubleValue 

Instance Property

# doubleValue

The value that indicates the current extent of the progress indicator.

macOS

``` source
@MainActor
var doubleValue: Double { get set }
```

## Discussion

By default, a determinate progress indicator goes from `0.0` to `100.0`. If the progress bar has advanced halfway across the view, this value would be `50.0`.

An indeterminate progress indicator does not use this value.

## See Also

### Advancing the progress bar

func increment(by: Double)

Advances the progress bar of a determinate progress indicator by the specified amount.

var minValue: Double

The minimum value for the progress indicator.

var maxValue: Double

The maximum value for the progress indicator.

