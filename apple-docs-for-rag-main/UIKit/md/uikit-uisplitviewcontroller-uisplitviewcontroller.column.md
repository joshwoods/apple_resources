

- UIKit
- UISplitViewController
-  UISplitViewController.Column 

Enumeration

# UISplitViewController.Column

Constants that describe the columns within the split view interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum Column
```

## Topics

### Constants

case primary

The column for the primary view controller.

case supplementary

The column for the supplementary view controller.

case secondary

The column for the secondary, or detail, view controller.

case compact

The column for the view controller that’s shown when the split view controller is collapsed.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the child view controllers

func setViewController(UIViewController?, for: UISplitViewController.Column)

Presents the provided view controller in the specified column of the split view interface.

func viewController(for: UISplitViewController.Column) -> UIViewController?

Returns the view controller associated with the specified column of the split view interface.

var viewControllers: [UIViewController]

The array of view controllers the split view controller manages.

