

- SwiftUI
- UIHostingController
-  preferredStatusBarUpdateAnimation 

Instance Property

# preferredStatusBarUpdateAnimation

The animation style to use when hiding or showing the status bar for this view controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
override dynamic var preferredStatusBarUpdateAnimation: UIStatusBarAnimation { get }
```

## See Also

### Configuring the status bar

var preferredStatusBarStyle: UIStatusBarStyle

The preferred status bar style for the view controller.

var prefersStatusBarHidden: Bool

A Boolean value that indicates whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarStyle: UIViewController?

var childForStatusBarHidden: UIViewController?

