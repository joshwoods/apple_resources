

- Multipeer Connectivity
- MCBrowserViewController
-  session 

Instance Property

# session

The multipeer session to which the invited peers are connected.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var session: MCSession { get }
```

## Discussion

This value is set when you initialize the object, and cannot be changed later.

## See Also

### Initializing a Browser View Controller

convenience init(serviceType: String, session: MCSession)

Initializes a browser view controller using the provided service type and session.

init(browser: MCNearbyServiceBrowser, session: MCSession)

Initializes a browser view controller with the provided browser and session.

var delegate: (any MCBrowserViewControllerDelegate)?

The delegate object that handles browser-view-controller-related events.

var browser: MCNearbyServiceBrowser?

The browser object that is used for discovering peers.

