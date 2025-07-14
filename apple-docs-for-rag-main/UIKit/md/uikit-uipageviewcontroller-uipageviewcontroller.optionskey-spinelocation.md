

- UIKit
- UIPageViewController
- UIPageViewController.OptionsKey
-  spineLocation 

Type Property

# spineLocation

Location of the spine.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
static let spineLocation: UIPageViewController.OptionsKey
```

## Discussion

For possible values, see UIPageViewController.SpineLocation. A spine location is only valid if the transition style is UIPageViewController.TransitionStyle.pageCurl.

If the transition style is UIPageViewController.TransitionStyle.pageCurl, the default value for this property is UIPageViewController.SpineLocation.min; otherwise, the default is UIPageViewController.SpineLocation.none.

## See Also

### Page options

static let interPageSpacing: UIPageViewController.OptionsKey

Space between pages, in points.

