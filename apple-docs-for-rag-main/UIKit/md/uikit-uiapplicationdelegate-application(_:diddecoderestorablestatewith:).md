

- UIKit
- UIApplicationDelegate
-  application(\_:didDecodeRestorableStateWith:) 

Instance Method

# application(\_:didDecodeRestorableStateWith:)

Tells your delegate to restore any high-level state information as part of the state restoration process.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didDecodeRestorableStateWith coder: NSCoder
)
```

## Parameters 

`application`  

Your singleton app object.

`coder`  

The keyed archiver containing the app’s previously saved state information.

## Discussion

The state restoration system calls this method as the final step in the state restoration process. By the time this method is called, all other restorable objects will have been restored and put back into their previous state. You can use this method to read any high-level app data you saved in the application(_:willEncodeRestorableStateWith:) method and apply it to your app.

## See Also

### Managing app state restoration

func application(UIApplication, shouldSaveSecureApplicationState: NSCoder) -> Bool

Asks the delegate whether to securely preserve the app’s state.

func application(UIApplication, shouldRestoreSecureApplicationState: NSCoder) -> Bool

Asks the delegate whether to restore the app’s saved state.

func application(UIApplication, viewControllerWithRestorationIdentifierPath: [String], coder: NSCoder) -> UIViewController?

Asks the delegate to provide the specified view controller.

func application(UIApplication, willEncodeRestorableStateWith: NSCoder)

Tells your delegate to save any high-level state information at the beginning of the state preservation process.

class let stateRestorationBundleVersionKey: String

The version of your app responsible for creating the restoration archive.

class let stateRestorationSystemVersionKey: String

The version of the system on which your app created the restoration archive.

class let stateRestorationTimestampKey: String

The time your app created the restoration archive.

class let stateRestorationUserInterfaceIdiomKey: String

The user interface idiom that was in effect when your app created the restoration archive.

class let stateRestorationViewControllerStoryboardKey: String

A reference to the storyboard that contains the view controller.

