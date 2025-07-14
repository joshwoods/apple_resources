

- TVMLKit
- TVBrowserViewController
-  delegate 

Instance Property

# delegate

The object that acts as the delegate and handles callbacks for the browser view.

tvOS 13.0+

``` source
@MainActor
weak var delegate: (any TVBrowserViewControllerDelegate)? { get set }
```

## See Also

### Managing Interactions with the Browser

protocol TVBrowserViewControllerDelegate

Methods for detecting events and performing actions on the browser view.

