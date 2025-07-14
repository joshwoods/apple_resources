

- Foundation
- NSFilePresenter
-  presentedItemDidMove(to:) 

Instance Method

# presentedItemDidMove(to:)

Tells your object that the presented item moved or was renamed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func presentedItemDidMove(to newURL: URL)
```

## Parameters 

`newURL`  

The URL containing the new path to the presented item.

## Discussion

Use this method to update the value returned by the presentedItemURL property of your object.

## See Also

### Related Documentation

var presentedItemURL: URL?

The URL of the presented file or directory.

**Required**

### Handling Changes to Files

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

Tells your object to save any unsaved changes for the presented item.

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

Tells your object that its presented item is about to be deleted.

func presentedItemDidChange()

Tells your object that the presented item’s contents or attributes changed.

