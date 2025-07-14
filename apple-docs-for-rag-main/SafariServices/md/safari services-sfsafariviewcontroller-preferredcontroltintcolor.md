

- Safari Services
- SFSafariViewController
-  preferredControlTintColor 

Instance Property

# preferredControlTintColor

The color to tint the control buttons on the navigation bar and the toolbar.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
var preferredControlTintColor: UIColor? { get set }
```

## Discussion

This color preference is ignored if the view controller is in Private Browsing mode or displaying an antiphishing warning. After the view controller is presented, changes made are not reflected. Use `preferredControlTintColor` instead of setting the view’s tintColor property.

## See Also

### Configuring the View Controller

var configuration: SFSafariViewController.Configuration

A copy of the Safari view controller’s initialized configuration.

var dismissButtonStyle: SFSafariViewController.DismissButtonStyle

enum DismissButtonStyle

var preferredBarTintColor: UIColor?

The color to tint the background of the navigation bar and the toolbar.

