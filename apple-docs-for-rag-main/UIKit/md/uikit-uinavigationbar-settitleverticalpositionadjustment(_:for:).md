

- UIKit
- UINavigationBar
-  setTitleVerticalPositionAdjustment(\_:for:) 

Instance Method

# setTitleVerticalPositionAdjustment(\_:for:)

Sets the title’s vertical position adjustment for given bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTitleVerticalPositionAdjustment(
    _ adjustment: CGFloat,
    for barMetrics: UIBarMetrics
)
```

## Parameters 

`adjustment`  

The title’s vertical position adjustment for `barMetrics`.

`barMetrics`  

A bar metrics constant.

## See Also

### Configuring the title

var titleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s title text.

var largeTitleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s large title text.

func titleVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the title’s vertical position adjustment for given bar metrics.

