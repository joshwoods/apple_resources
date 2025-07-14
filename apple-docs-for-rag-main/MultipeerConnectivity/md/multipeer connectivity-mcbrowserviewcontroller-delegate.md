

- Multipeer Connectivity
- MCBrowserViewController
-  delegate 

Instance Property

# delegate

The delegate object that handles browser-view-controller-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any MCBrowserViewControllerDelegate)? { get set }
```

## Discussion

A browser view controller notifies the delegate:

- When the user presses the “Done” button, which is enabled when the specified minimum number of peers are connected in a session.

- When the user cancels the view controller.

Also, as new peers are discovered, the delegate can choose whether to present them in the user interface.

## See Also

### Initializing a Browser View Controller

convenience init(serviceType: String, session: MCSession)

Initializes a browser view controller using the provided service type and session.

init(browser: MCNearbyServiceBrowser, session: MCSession)

Initializes a browser view controller with the provided browser and session.

var browser: MCNearbyServiceBrowser?

The browser object that is used for discovering peers.

var session: MCSession

The multipeer session to which the invited peers are connected.

