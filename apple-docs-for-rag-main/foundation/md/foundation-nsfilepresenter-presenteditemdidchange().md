

- Foundation
- NSFilePresenter
-  presentedItemDidChange() 

Instance Method

# presentedItemDidChange()

Tells your object that the presented item’s contents or attributes changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func presentedItemDidChange()
```

## Discussion

You can use this method to update your internal data structures to reflect the changes to the presented item. This method reports both changes to the file’s contents, such as the data in a file or the files in a directory, or the attributes of the item, such as whether the Hide extension checkbox of a file was toggled.

Because this method notifies you of both attribute and content changes, you might want to check the modification date before needlessly rereading the contents of a file. To do that, you must store the date when your object last made changes to the file and compare that date with the item’s current modification date. Use the coordinate(readingItemAt:options:error:byAccessor:) method of a file coordinator to ensure exclusive access to the file when reading the current modification date.

## See Also

### Handling Changes to Files

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

Tells your object to save any unsaved changes for the presented item.

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

Tells your object that its presented item is about to be deleted.

func presentedItemDidMove(to: URL)

Tells your object that the presented item moved or was renamed.

