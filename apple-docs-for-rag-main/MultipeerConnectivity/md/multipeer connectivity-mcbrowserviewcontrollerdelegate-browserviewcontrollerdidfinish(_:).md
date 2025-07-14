

- Multipeer Connectivity
- MCBrowserViewControllerDelegate
-  browserViewControllerDidFinish(\_:) 

Instance Method

# browserViewControllerDidFinish(\_:)

Called when the browser view controller is dismissed with peers connected in a session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func browserViewControllerDidFinish(_ browserViewController: MCBrowserViewController)
```

**Required**

## Parameters 

`browserViewController`  

The view controller that was dismissed.

## Discussion

This call is intended to inform your app that the user has connected with nearby peers in a session and that the browser view controller has been dismissed. Upon receiving this delegate method call, your app must call dismiss(animated:completion:) to dismiss the view controller. Your app can also begin sending data to any connected peers, and should resume any UI updates that it may have temporarily suspended while the view controller was onscreen.

## See Also

### User Action Notifications

func browserViewControllerWasCancelled(MCBrowserViewController)

Called when the user cancels the browser view controller.

**Required**

