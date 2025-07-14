

- AppKit
- NSProgressIndicator
-  increment(by:) 

Instance Method

# increment(by:)

Advances the progress bar of a determinate progress indicator by the specified amount.

macOS

``` source
@MainActor
func increment(by delta: Double)
```

## Parameters 

`delta`  

The amount by which to increment the progress bar. For example, if you want to advance a progress bar from 0.0 to 100.0 in 20 steps, you would invoke increment(by:) 20 times with a delta value of 5.0.

## See Also

### Advancing the progress bar

var doubleValue: Double

The value that indicates the current extent of the progress indicator.

var minValue: Double

The minimum value for the progress indicator.

var maxValue: Double

The maximum value for the progress indicator.

