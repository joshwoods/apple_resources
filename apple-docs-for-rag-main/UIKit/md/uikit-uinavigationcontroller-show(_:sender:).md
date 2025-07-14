

- UIKit
- UINavigationController
-  show(\_:sender:) 

Instance Method

# show(\_:sender:)

Presents the specified view controller in the navigation interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func show(
    _ vc: UIViewController,
    sender: Any?
)
```

## Parameters 

`vc`  

The view controller to display.

`sender`  

The object that made the request to show the view controller.

## Discussion

This method pushes `vc` onto the navigation stack in a similar way as the pushViewController(_:animated:) method. You can call this method directly if you want but typically this method is called from elsewhere in the view controller hierarchy when a new view controller needs to be shown.

The Show segue uses this method to display a new view controller.

