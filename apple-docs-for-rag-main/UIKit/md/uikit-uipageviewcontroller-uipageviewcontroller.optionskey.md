

- UIKit
- UIPageViewController
-  UIPageViewController.OptionsKey 

Structure

# UIPageViewController.OptionsKey

Keys for creating the page view controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct OptionsKey
```

## Topics

### Page options

static let interPageSpacing: UIPageViewController.OptionsKey

Space between pages, in points.

static let spineLocation: UIPageViewController.OptionsKey

Location of the spine.

### Initializers

init(rawValue: String)

Creates a page view controller options structure with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a page view controller

init(transitionStyle: UIPageViewController.TransitionStyle, navigationOrientation: UIPageViewController.NavigationOrientation, options: [UIPageViewController.OptionsKey : Any]?)

Initializes a newly created page view controller.

init?(coder: NSCoder)

Creates a page view controller from data in an unarchiver.

