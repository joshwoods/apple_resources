

- UIKit
- UIViewController
-  decodeRestorableState(with:) 

Instance Method

# decodeRestorableState(with:)

Decodes and restores state-related information for the view controller.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func decodeRestorableState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object to use to decode the state of the view.

## Mentioned in 

About the UI restoration process

## Discussion

Do not call this method directly. The system calls this method during the state restoration process so that you can restore your view controller to its previous state.

If your app supports state restoration, override this method for any view controllers for which you also overrode the encodeRestorableState(with:) method. Your implementation of this method should use any saved state information to restore the view controller to its previous configuration. If your encodeRestorableState(with:) method called `super`, this method should similarly call `super` at some point in its implementation.

## See Also

### Managing state restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

var restorationIdentifier: String?

The identifier that determines whether the view controller supports state restoration.

var restorationClass: (any UIViewControllerRestoration.Type)?

The class responsible for recreating this view controller when restoring the app’s state.

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the view controller.

func applicationFinishedRestoringState()

Called on restored view controllers after other object decoding is complete.

