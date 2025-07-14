

- Multipeer Connectivity
- MCBrowserViewControllerDelegate
-  browserViewControllerWasCancelled(\_:) 

Instance Method

# browserViewControllerWasCancelled(\_:)

Called when the user cancels the browser view controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func browserViewControllerWasCancelled(_ browserViewController: MCBrowserViewController)
```

**Required**

## Parameters 

`browserViewController`  

The browser view controller that was canceled.

## Discussion

This call is intended to inform your app that the view controller has been dismissed because the user canceled the discovery process and is no longer interested in creating a communication session.

When your app receives this delegate method call, your app must call dismiss(animated:completion:) to dismiss the view controller. Then, your app should handle the cancelation in whatever way is appropriate for your app, and then resume any UI updates that it may have temporarily suspended while the view controller was onscreen.

## See Also

### User Action Notifications

func browserViewControllerDidFinish(MCBrowserViewController)

Called when the browser view controller is dismissed with peers connected in a session.

**Required**

