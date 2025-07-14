

- UIKit
- UIApplicationDelegate
-  application(\_:willEncodeRestorableStateWith:) 

Instance Method

# application(\_:willEncodeRestorableStateWith:)

Tells your delegate to save any high-level state information at the beginning of the state preservation process.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    willEncodeRestorableStateWith coder: NSCoder
)
```

## Parameters 

`application`  

Your singleton app object.

`coder`  

The keyed archiver in which to write any state information.

## Mentioned in 

About the UI preservation process

## Discussion

The state preservation system calls this method at the beginning of the preservation process. This is your opportunity to add any app-level information to state information. For example, you might use this method to write version information or the high-level configuration of your app.

Important

This method is not a substitute for saving your app’s data structures persistently to disk. You should continue to save your app’s actual data to iCloud or the local file system using existing techniques. This method is intended only for saving configuration state or other information related to your app’s user interface. You should consider the data in the coder as purgeable and be prepared for it to be unavailable during subsequent launches.

Your implementation of this method can encode restorable view and view controller objects that it needs to reference. Encoding a restorable view or view controller writes that object’s restoration identifier to the coder. (That identifier is used during the decode process to locate the new version of the object.) If the view or view controller defines a encodeRestorableState(with:) method, that method is also called at some point so that the object can encode its own state.

Apart from views and view controllers, other objects follow the normal serialization process and must adopt the NSCoding protocol before they can be encoded. Encoding such objects embeds the object’s contents in the archive directly. During the decode process, a new object is created and initialized with the data from the archive.

## See Also

### Managing app state restoration

func application(UIApplication, shouldSaveSecureApplicationState: NSCoder) -> Bool

Asks the delegate whether to securely preserve the app’s state.

func application(UIApplication, shouldRestoreSecureApplicationState: NSCoder) -> Bool

Asks the delegate whether to restore the app’s saved state.

func application(UIApplication, viewControllerWithRestorationIdentifierPath: [String], coder: NSCoder) -> UIViewController?

Asks the delegate to provide the specified view controller.

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

