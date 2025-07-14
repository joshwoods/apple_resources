

- Foundation
- NSFilePresenter
-  accommodatePresentedSubitemDeletion(at:completionHandler:) 

Instance Method

# accommodatePresentedSubitemDeletion(at:completionHandler:)

Tells the delegate that some entity wants to delete an item that is inside of a presented directory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func accommodatePresentedSubitemDeletion(
    at url: URL,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
optional func accommodatePresentedSubitemDeletion(at url: URL) async throws
```

## Parameters 

`url`  

The URL of the item being deleted from the presented directory. The item need not be at the top level of the presented directory but may itself be inside a nested subdirectory.

`completionHandler`  

The Block object to call after updating your data structures. Pass `nil` to the block’s `errorOrNil` parameter if you were able to successfully prepare for the deletion of the item. Pass an error object if your object could not prepare itself properly.

## Discussion

This method is relevant for applications that present directories. This might occur if the delegate manages the contents of a directory or manages a file that is implemented as a file package. When called, your implementation of this method should take whatever actions needed to update your application to handle the deletion of the specified file.

Important

If you implement this method, you must execute the block in the `completionHandler` parameter at the end of your implementation. The system waits for you to execute that block before allowing the other object to delete the item at the specified URL. Therefore, failure to execute the block could stall threads in your application or in other processes.

## See Also

### Handling Changes to a Presented Directory

func presentedSubitemDidAppear(at: URL)

Tells the delegate that an item was added to the presented directory.

func presentedSubitem(at: URL, didMoveTo: URL)

Tells the delegate that an item in the presented directory moved to a new location.

func presentedSubitemDidChange(at: URL)

Tells the delegate that the contents or attributes of the specified item changed.

