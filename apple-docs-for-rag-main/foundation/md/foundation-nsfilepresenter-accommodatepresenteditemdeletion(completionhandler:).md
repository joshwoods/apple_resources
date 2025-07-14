

- Foundation
- NSFilePresenter
-  accommodatePresentedItemDeletion(completionHandler:) 

Instance Method

# accommodatePresentedItemDeletion(completionHandler:)

Tells your object that its presented item is about to be deleted.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func accommodatePresentedItemDeletion(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
optional func accommodatePresentedItemDeletion() async throws
```

## Parameters 

`completionHandler`  

The Block object to call after updating your data structures. Pass `nil` to the block’s `errorOrNil` parameter if you were able to successfully prepare for the deletion of the item. Pass an error object if your object could not prepare itself properly.

## Discussion

A file coordinator calls this method when your object’s presented item is about to be deleted. You can use this method to perform any actions that are needed to prepare for the deletion. For example, document objects typically use this method to close the document.

Important

If you implement this method, you must execute the block in the `completionHandler` parameter at the end of your implementation. The system waits for you to execute that block before allowing the other object to delete the file or directory. Therefore, failure to execute the block could stall threads in your application or other processes.

## See Also

### Handling Changes to Files

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

Tells your object to save any unsaved changes for the presented item.

func presentedItemDidMove(to: URL)

Tells your object that the presented item moved or was renamed.

func presentedItemDidChange()

Tells your object that the presented item’s contents or attributes changed.

