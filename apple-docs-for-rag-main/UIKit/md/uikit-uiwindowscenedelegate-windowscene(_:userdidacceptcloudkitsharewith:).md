

- UIKit
- UIWindowSceneDelegate
-  windowScene(\_:userDidAcceptCloudKitShareWith:) 

Instance Method

# windowScene(\_:userDidAcceptCloudKitShareWith:)

Tells the delegate that the window scene now has access to shared information in CloudKit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func windowScene(
    _ windowScene: UIWindowScene,
    userDidAcceptCloudKitShareWith cloudKitShareMetadata: CKShareMetadata
)
```

## Parameters 

`windowScene`  

The window scene object receiving the metadata.

`cloudKitShareMetadata`  

Information about the CloudKit data that is now available to the app. Use this object to retrieve information about the CKShare object and the associated records.

## Discussion

Use this method to respond to a CloudKit Sharing invitation. In your implementation, accept the share by scheduling a CKAcceptSharesOperation object that contains the metadata object in the `cloudKitShareMetadata` parameter. After your operation object finishes successfully, you can begin fetching records and incorporating the resulting data into your app. Alternatively, if your app uses Core Data and NSPersistentCloudKitContainer, accept the share by calling the container’s acceptShareInvitations(from:into:completion:) method.

Note

To use this method in a SwiftUI app, you must first add scene and application delegates to your project and configure your app to use them. For more information, see Accepting Share Invitations in a SwiftUI App.

The system calls this method only when your app is running and has an existing scene. If your app isn’t running, the system includes the share metadata in the UIScene.ConnectionOptions object it passes to the init(session:connectionOptions:) method when it creates your app’s first scene.

## See Also

### Performing tasks

func windowScene(UIWindowScene, performActionFor: UIApplicationShortcutItem, completionHandler: (Bool) -> Void)

Asks the delegate to perform the user-selected action.

