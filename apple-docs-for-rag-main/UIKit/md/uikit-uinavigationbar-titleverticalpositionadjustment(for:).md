

- UIKit
- UINavigationBar
-  titleVerticalPositionAdjustment(for:) 

Instance Method

# titleVerticalPositionAdjustment(for:)

Returns the title’s vertical position adjustment for given bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func titleVerticalPositionAdjustment(for barMetrics: UIBarMetrics) -> CGFloat
```

## Parameters 

`barMetrics`  

A bar metrics constant.

## Return Value

The title’s vertical position adjustment for `barMetrics`.

## See Also

### Configuring the title

var titleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s title text.

var largeTitleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s large title text.

func setTitleVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the title’s vertical position adjustment for given bar metrics.

