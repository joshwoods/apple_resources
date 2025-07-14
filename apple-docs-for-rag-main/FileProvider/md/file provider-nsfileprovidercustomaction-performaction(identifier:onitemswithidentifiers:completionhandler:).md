

- File Provider
- NSFileProviderCustomAction
-  performAction(identifier:onItemsWithIdentifiers:completionHandler:) 

Instance Method

# performAction(identifier:onItemsWithIdentifiers:completionHandler:)

Tells the File Provider extension to perform a custom action.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func performAction(
    identifier actionIdentifier: NSFileProviderExtensionActionIdentifier,
    onItemsWithIdentifiers itemIdentifiers: [NSFileProviderItemIdentifier],
    completionHandler: @escaping ((any Error)?) -> Void
) -> Progress
```

**Required**

## Parameters 

`actionIdentifier`  

The identifier for the requested custom action from the extension’s `Info.plist` file.

`itemIdentifiers`  

A list of item identifiers affected by the action.

`completionHandler`  

A block that you call after completing the specified action. You pass the following parameters:

error  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Return Value

An item that tracks your extension’s progress.

## Discussion

Define the custom actions in the File Provider Extension’s `Info.plist` file, under the `NSExtensionFileProviderActions` key. The format of this key is identical to actions defined for a File Provider UI extension. For more information, see `Adding Actions to the Context Menu`.

