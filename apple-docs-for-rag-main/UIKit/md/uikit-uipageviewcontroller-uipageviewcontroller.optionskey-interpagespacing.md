

- UIKit
- UIPageViewController
- UIPageViewController.OptionsKey
-  interPageSpacing 

Type Property

# interPageSpacing

Space between pages, in points.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static let interPageSpacing: UIPageViewController.OptionsKey
```

## Discussion

The value should be a CGFloat wrapped in an instance of NSNumber. The default value is zero. An inter-page spacing is only valid if the transition style is UIPageViewController.TransitionStyle.scroll.

## See Also

### Page options

static let spineLocation: UIPageViewController.OptionsKey

Location of the spine.

