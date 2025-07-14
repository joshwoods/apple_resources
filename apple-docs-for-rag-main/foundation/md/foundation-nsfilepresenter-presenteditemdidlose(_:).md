

- Foundation
- NSFilePresenter
-  presentedItemDidLose(\_:) 

Instance Method

# presentedItemDidLose(\_:)

Tells the delegate that a version of the file or file package was removed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func presentedItemDidLose(_ version: NSFileVersion)
```

## Parameters 

`version`  

The file version object containing information about the version that was removed.

## Discussion

Your delegate can use this method to determine how to handle the loss of the specified file version. You can try to revert the presented document to a previous version or you might want to prompt the user about how to proceed.

## See Also

### Responding to Version Changes

func presentedItemDidGain(NSFileVersion)

Tells the delegate that a new version of the file or file package was added.

func presentedItemDidResolveConflict(NSFileVersion)

Tells the delegate that some other entity resolved a version conflict for the presenter’s file or file package.

func presentedSubitem(at: URL, didGain: NSFileVersion)

Tells the delegate that the item inside the presented directory gained a new version.

func presentedSubitem(at: URL, didLose: NSFileVersion)

Tells the delegate that the item inside the presented directory lost an existing version.

func presentedSubitem(at: URL, didResolve: NSFileVersion)

Tells the delegate that the item inside the presented directory had a version conflict resolved by an outside entity.

