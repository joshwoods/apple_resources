

- Multipeer Connectivity
- MCBrowserViewController
-  init(browser:session:) 

Initializer

# init(browser:session:)

Initializes a browser view controller with the provided browser and session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init(
    browser: MCNearbyServiceBrowser,
    session: MCSession
)
```

## Parameters 

`browser`  

An object that the browser view controller uses for browsing. This is usually an instance of `MCNearbyServiceBrowser`. However, if your app is using a custom discovery scheme, you can instead pass any custom subclass that calls the methods defined in the MCNearbyServiceBrowserDelegate protocol on its delegate when peers are found and lost.

Important

If you want the browser view controller to manage the browsing process, the browser object must not be actively browsing, and its delegate must be `nil`.

`session`  

The multipeer session into which the invited peers are connected.

## Return Value

Returns an initialized object, or `nil` if an error occurred.

## Discussion

This method throws an exception if the `browser` or `session` parameters do not contain valid objects.

## See Also

### Initializing a Browser View Controller

convenience init(serviceType: String, session: MCSession)

Initializes a browser view controller using the provided service type and session.

var delegate: (any MCBrowserViewControllerDelegate)?

The delegate object that handles browser-view-controller-related events.

var browser: MCNearbyServiceBrowser?

The browser object that is used for discovering peers.

var session: MCSession

The multipeer session to which the invited peers are connected.

