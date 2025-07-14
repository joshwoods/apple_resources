

- UIKit
- UIApplicationDelegate
-  application(\_:shouldRestoreSecureApplicationState:) 

Instance Method

# application(\_:shouldRestoreSecureApplicationState:)

Asks the delegate whether to restore the app’s saved state.

iOS 13.2+iPadOS 13.2+Mac Catalyst 13.2+tvOS 13.2+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    shouldRestoreSecureApplicationState coder: NSCoder
) -> Bool
```

## Parameters 

`application`  

The singleton app object.

`coder`  

A keyed archiver containing the app’s previously saved state. The coder’s requiresSecureCoding property is set to true, and any objects you decode must adopt NSSecureCoding.

## Return Value

true to restore the app’s saved state; otherwise, false.

## Discussion

Apps must implement both this method and application(_:shouldSaveSecureApplicationState:) for state preservation to occur.

Use the information from the provided coder to determine whether to proceed with state restoration. For example, you might return false if the data in the coder is from an earlier version of your app and you can’t restore it safely. Any objects you decode from the coder must adopt the NSSecureCoding protocol.

This method supersedes application(_:shouldRestoreApplicationState:). If your delegate implements both methods, the system only calls this one.

## See Also

### Managing app state restoration

func application(UIApplication, shouldSaveSecureApplicationState: NSCoder) -> Bool

Asks the delegate whether to securely preserve the app’s state.

func application(UIApplication, viewControllerWithRestorationIdentifierPath: [String], coder: NSCoder) -> UIViewController?

Asks the delegate to provide the specified view controller.

func application(UIApplication, willEncodeRestorableStateWith: NSCoder)

Tells your delegate to save any high-level state information at the beginning of the state preservation process.

func application(UIApplication, didDecodeRestorableStateWith: NSCoder)

Tells your delegate to restore any high-level state information as part of the state restoration process.

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

