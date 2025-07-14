

- UIKit
- UIScreen
-  wantsSoftwareDimming 

Instance Property

# wantsSoftwareDimming

A Boolean value that indicates whether the screen may be dimmed lower than the hardware is normally capable of by emulating it in software.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+

``` source
@MainActor
var wantsSoftwareDimming: Bool { get set }
```

## Discussion

The default value is false. Enabling it may cause a loss in performance.

## See Also

### Managing brightness

var brightness: CGFloat

The brightness level of the screen.

