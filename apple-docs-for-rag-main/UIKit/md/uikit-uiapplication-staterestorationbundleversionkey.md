

- UIKit
- UIApplication
-  stateRestorationBundleVersionKey 

Type Property

# stateRestorationBundleVersionKey

The version of your app responsible for creating the restoration archive.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class let stateRestorationBundleVersionKey: String
```

## Discussion

The value of this key is an NSString object that identifies the version of your app (as obtained from the `CFBundleVersion` key of your app’s `Info.plist` file) that was present when the state information was saved. You can use the value of this key to help make choices about how to proceed during state restoration. For example, if the key indicates that the state is associated with an older version of your app, you might want to avoid restoring the previous state altogether or modify the restoration process more significantly.

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

func application(UIApplication, didDecodeRestorableStateWith: NSCoder)

Tells your delegate to restore any high-level state information as part of the state restoration process.

class let stateRestorationSystemVersionKey: String

The version of the system on which your app created the restoration archive.

class let stateRestorationTimestampKey: String

The time your app created the restoration archive.

class let stateRestorationUserInterfaceIdiomKey: String

The user interface idiom that was in effect when your app created the restoration archive.

class let stateRestorationViewControllerStoryboardKey: String

A reference to the storyboard that contains the view controller.

