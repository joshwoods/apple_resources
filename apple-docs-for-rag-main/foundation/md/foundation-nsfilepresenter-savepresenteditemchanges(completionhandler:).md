

- Foundation
- NSFilePresenter
-  savePresentedItemChanges(completionHandler:) 

Instance Method

# savePresentedItemChanges(completionHandler:)

Tells your object to save any unsaved changes for the presented item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func savePresentedItemChanges(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
optional func savePresentedItemChanges() async throws
```

## Parameters 

`completionHandler`  

The Block object to call after you save your changes. If you saved your changes successfully, pass `nil` for the block’s `errorOrNil` parameter; otherwise, pass an error object indicating why the changes could not be saved.

## Discussion

The file coordinator calls this method to ensure that all objects trying to access the file or directory see the same contents. Implement this method if your object can change the presented item in a way that requires you to write those changes back to disk. If your presenter object does not make changes that need to be saved, you do not need to implement this method.

Important

If you implement this method, you must execute the block in the `completionHandler` parameter at the end of your implementation. The system waits for you to execute that block before allowing other objects to operate on the file. Therefore, failure to execute the block could stall threads in your application or other processes.

## See Also

### Handling Changes to Files

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

Tells your object that its presented item is about to be deleted.

func presentedItemDidMove(to: URL)

Tells your object that the presented item moved or was renamed.

func presentedItemDidChange()

Tells your object that the presented item’s contents or attributes changed.

