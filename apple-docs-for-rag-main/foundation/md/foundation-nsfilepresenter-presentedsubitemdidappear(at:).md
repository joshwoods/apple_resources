

- Foundation
- NSFilePresenter
-  presentedSubitemDidAppear(at:) 

Instance Method

# presentedSubitemDidAppear(at:)

Tells the delegate that an item was added to the presented directory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func presentedSubitemDidAppear(at url: URL)
```

## Parameters 

`url`  

The URL of the item being added to the presented directory. The item need not be at the top level of the presented directory but may itself be inside a nested subdirectory.

## Discussion

This method is relevant for applications that present directories. This might occur if the delegate manages the contents of a directory or manages a file that is implemented as a file package. Your implementation of this method should take whatever actions necessary to incorporate the new file or directory into the presented content. For example, you might add the new item to your application’s data structures and refresh your user interface.

If the presented directory is a file package, the system calls the presentedItemDidChange() method if your delegate does not implement this method.

## See Also

### Handling Changes to a Presented Directory

func accommodatePresentedSubitemDeletion(at: URL, completionHandler: ((any Error)?) -> Void)

Tells the delegate that some entity wants to delete an item that is inside of a presented directory.

func presentedSubitem(at: URL, didMoveTo: URL)

Tells the delegate that an item in the presented directory moved to a new location.

func presentedSubitemDidChange(at: URL)

Tells the delegate that the contents or attributes of the specified item changed.

