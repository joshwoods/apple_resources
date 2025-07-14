

- UIKit
- UIWindowSceneDelegate
-  windowScene(\_:performActionFor:completionHandler:) 

Instance Method

# windowScene(\_:performActionFor:completionHandler:)

Asks the delegate to perform the user-selected action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func windowScene(
    _ windowScene: UIWindowScene,
    performActionFor shortcutItem: UIApplicationShortcutItem,
    completionHandler: @escaping (Bool) -> Void
)
```

``` source
@MainActor
optional func windowScene(
    _ windowScene: UIWindowScene,
    performActionFor shortcutItem: UIApplicationShortcutItem
) async -> Bool
```

## Parameters 

`windowScene`  

The window scene object receiving the shortcut item.

`shortcutItem`  

The action selected by the user. Your app defines the actions that it supports, and the user chooses from among those actions. For information about how to create and configure shortcut items for your app, see UIApplicationShortcutItem.

`completionHandler`  

A handler block to call after you complete the action. This block has no return value and takes the following parameter:

succeeded  
A Boolean value indicating whether you successfully completed the specified action. Specify true if you completed the action or false if you didn’t.

## Discussion

When the user selects one of your app’s shortcut items, use this method to perform the selected action. After you finish the action, execute the specified `completionHandler` block to report your success or failure in performing the action.

## See Also

### Performing tasks

func windowScene(UIWindowScene, userDidAcceptCloudKitShareWith: CKShareMetadata)

Tells the delegate that the window scene now has access to shared information in CloudKit.

