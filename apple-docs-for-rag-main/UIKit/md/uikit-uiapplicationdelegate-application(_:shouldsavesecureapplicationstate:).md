

- UIKit
- UIApplicationDelegate
-  application(\_:shouldSaveSecureApplicationState:) 

Instance Method

# application(\_:shouldSaveSecureApplicationState:)

Asks the delegate whether to securely preserve the app’s state.

iOS 13.2+iPadOS 13.2+Mac Catalyst 13.2+tvOS 13.2+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    shouldSaveSecureApplicationState coder: NSCoder
) -> Bool
```

## Parameters 

`application`  

The singleton app object.

`coder`  

A keyed archiver where you can store high-level state information. The coder’s requiresSecureCoding property is set to true, and any objects you encode must adopt NSSecureCoding.

## Return Value

true to securely preserve the app’s state; otherwise, false.

## Discussion

Apps must implement both this method and application(_:shouldRestoreSecureApplicationState:) for state preservation to occur.

Your implementation of this method should return true each time UIKit attempts to preserve the state of your app. You can temporarily disable state preservation by returning false, which you may want to do during testing, for example.

You can add version information or any other contextual data to the provided coder as necessary. During restoration, you can use that information to determine whether to proceed with restoring your app to its previous state. Any objects you add to the coder must adopt the NSSecureCoding protocol.

This method supersedes application(_:shouldSaveApplicationState:). If your delegate implements both methods, the system only calls this one.

## See Also

### Managing app state restoration

func application(UIApplication, shouldRestoreSecureApplicationState: NSCoder) -> Bool

Asks the delegate whether to restore the app’s saved state.

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

