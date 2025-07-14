

- AppKit
- NSDocument
-  presentedItemDidResolveConflict(\_:) 

Instance Method

# presentedItemDidResolveConflict(\_:)

macOS 10.7+

``` source
nonisolated
func presentedItemDidResolveConflict(_ version: NSFileVersion)
```

## See Also

### Instance Methods

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

func presentedItemDidChange()

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

func presentedItemDidGain(NSFileVersion)

func presentedItemDidLose(NSFileVersion)

func presentedItemDidMove(to: URL)

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

