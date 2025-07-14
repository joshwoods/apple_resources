

- UIKit
- UIApplication
-  registerObject(forStateRestoration:restorationIdentifier:) 

Type Method

# registerObject(forStateRestoration:restorationIdentifier:)

Registers a custom object for use with the state restoration system.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func registerObject(
    forStateRestoration object: any UIStateRestoring,
    restorationIdentifier: String
)
```

## Parameters 

`object`  

The object to be registered with the restoration archive. The object must adopt the UIStateRestoring protocol. This parameter must not be `nil`.

`restorationIdentifier`  

The restoration identifier for the object. UIKit uses this parameter to distinguish the object from other objects in the archive. This parameter must not be `nil`.

## Mentioned in 

About the UI preservation process

## Discussion

You use this method to register objects that you want to save as part of the overall state restoration process. Registering the object makes it available for inclusion in the restoration archive but does not automatically include it. To include the object, refer to it from one of your other interface objects. For example, you might write out a reference to the object from the encodeRestorableState(with:) method of one of your view controllers.

## See Also

### Managing state restoration

func extendStateRestoration()

Tells the app that your code is restoring state asynchronously.

func completeStateRestoration()

Tells the app that your code has finished any asynchronous state restoration.

func ignoreSnapshotOnNextApplicationLaunch()

Prevents the app from using the recent snapshot image during the next launch cycle.

