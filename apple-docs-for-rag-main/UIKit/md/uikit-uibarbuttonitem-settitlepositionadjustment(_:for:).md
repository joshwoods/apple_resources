

- UIKit
- UIBarButtonItem
-  setTitlePositionAdjustment(\_:for:) 

Instance Method

# setTitlePositionAdjustment(\_:for:)

Sets the title offset for specified bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTitlePositionAdjustment(
    _ adjustment: UIOffset,
    for barMetrics: UIBarMetrics
)
```

## Parameters 

`adjustment`  

The title offset for `barMetrics`.

`barMetrics`  

Bar metrics.

## Discussion

This offset is used to adjust the position of a title (if any) within a bordered bar button.

## See Also

### Customizing the title placement

func titlePositionAdjustment(for: UIBarMetrics) -> UIOffset

Returns the title offset for specified bar metrics.

