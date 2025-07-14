

- UIKit
- UIBarButtonItem
-  titlePositionAdjustment(for:) 

Instance Method

# titlePositionAdjustment(for:)

Returns the title offset for specified bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func titlePositionAdjustment(for barMetrics: UIBarMetrics) -> UIOffset
```

## Parameters 

`barMetrics`  

Bar metrics.

## Return Value

The title offset for `barMetrics`.

## Discussion

This offset is used to adjust the position of a title (if any) within a bordered bar button.

## See Also

### Customizing the title placement

func setTitlePositionAdjustment(UIOffset, for: UIBarMetrics)

Sets the title offset for specified bar metrics.

