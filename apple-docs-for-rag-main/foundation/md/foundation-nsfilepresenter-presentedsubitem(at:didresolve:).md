

- Foundation
- NSFilePresenter
-  presentedSubitem(at:didResolve:) 

Instance Method

# presentedSubitem(at:didResolve:)

Tells the delegate that the item inside the presented directory had a version conflict resolved by an outside entity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func presentedSubitem(
    at url: URL,
    didResolve version: NSFileVersion
)
```

## Parameters 

`url`  

The URL of the item inside the presented directory that was in conflict. The item need not be at the top level of the presented directory but may itself be inside a nested subdirectory.

`version`  

The version object containing the conflicting change.

## Discussion

Your delegate can use this method to respond to the resolution of a version conflict by a different file presenter. This might occur if a version of your application running on another device resolves the conflict first. You might then use this method to update your user interface to indicate that there is no longer a conflict.

## See Also

### Responding to Version Changes

func presentedItemDidGain(NSFileVersion)

Tells the delegate that a new version of the file or file package was added.

func presentedItemDidLose(NSFileVersion)

Tells the delegate that a version of the file or file package was removed.

func presentedItemDidResolveConflict(NSFileVersion)

Tells the delegate that some other entity resolved a version conflict for the presenter’s file or file package.

func presentedSubitem(at: URL, didGain: NSFileVersion)

Tells the delegate that the item inside the presented directory gained a new version.

func presentedSubitem(at: URL, didLose: NSFileVersion)

Tells the delegate that the item inside the presented directory lost an existing version.

